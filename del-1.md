# Idiomatisk Python - del 1 av 3

Alle språk har sine særegenheter, med sine styrker og svakheter. 
Bak et hvert språk ligger en filosofi—en tanke om hvordan språket bør brukes.
Dette reflekteres gjerne i hvilke konstruksjoner og konsepter språket tilbyr.
For å skrive pen kode er det viktig å kjenne og bruke språkets særegenheter; de uttrykk som er idiomatiske for språket.

Dette er første del i en serie på 3 bloggposter om idiomatisk Python.
I denne delen tar vi for oss begrepet *Pythonisk kode* og diskuterer en rekke konsepter som underbygger dette.
Del 2 kommer til å ta for seg sekvenser og lister, og gå igjennom hvordan Python legger opp til å arbeide med slike på en god måte.
I den siste posten skal vi ta en nærmere titt på funksjoner i Python, og hva disse kan brukes til.

Bloggpostene er basert på [del 2](http://magnhaug.github.com/BEKK-Python-Kurs/slides/del2.html#1) av BEKKs [kursserie om Python](https://github.com/bekkopen/BEKK-Python-Kurs) på NTNU, og er derfor beregnet på lesere som kjenner grunnleggende Python uten å være godt kjent med språket.

## Hva er Pythonisk kode?

Pythonisk kode er kode som bruker vanlige idiomer i Python på en god måte, i stedet for å implementere koden ved hjelp av konsepter og teknikker som er vanligere i andre språk.

Dette kan illustreres med et enkelt eksempel hentet fra Pythons [offesielle ordliste](http://docs.python.org/glossary.html#term-pythonic).
I mange språk er det vanlig å iterere over elementer i lister ved hjelp av en eksplisitt indeks og en for-løkke.

        for (int i=0; i<food.length; i++) {
            System.out.println(food[i]);
        }

Dette er også mulig i Python, og kan gjøres slik:

    for i in range(len(food)):
        print food[i]

I Python er det imidlertid et vanlig idiom å iterere over alle elementene i en sekvens direkte.
 
    for piece in food:
        print piece

Vi ser at koden umiddelbart blir enklere og penere, ved at vi kvitter oss med hele den forstyrrende indeksen.
Selv om dette er et overforenklet eksempel, illusterer det godt essensen i hva som menes med *pythonisk*.

Pythonisk kode er også tett knyttet opp mot filosofien om minimalisme og enkelhet som underbygger Python.

## The Zen of Python

Den beste beskrivelsen av denne Pythons filosofi er kanskje gitt i The Zen of Python:

    >> import this
    The Zen of Python, by Tim Peters

    Beautiful is better than ugly.
    Explicit is better than implicit.
    Simple is better than complex.
    Complex is better than complicated.
    Flat is better than nested.
    Sparse is better than dense.
    Readability counts.
    Special cases aren't special enough to break the rules.
    Although practicality beats purity.
    Errors should never pass silently.
    Unless explicitly silenced.
    In the face of ambiguity, refuse the temptation to guess.
    There should be one-- and preferably only one --obvious way to do it.
    Although that way may not be obvious at first unless you're Dutch.
    Now is better than never.
    Although never is often better than *right* now.
    If the implementation is hard to explain, it's a bad idea.
    If the implementation is easy to explain, it may be a good idea.
    Namespaces are one honking great idea -- let's do more of those!

For å oppsummere, det aller viktigste er at kode er enkel og uttrykksfull.
Vi ønsker kode som er så enkel å forstå at den blir vakker.

> *Programs must be written for people to read, and only incidentally for machines to execute.*  
> —Abelson & Sussman, Structure and Interpretation of Computer Programs

Dette oppnår vi i Python ved å kjenne språket, og bruke de konstruktene som tilbys på riktig måte.
Vil du lese mer, inneholder [denne stackoverflow-posten](http://stackoverflow.com/questions/228181/the-zen-of-python) diskusjoner og beskrivelser av hva som menes med mange uttrykkene i Zen of Python.

La oss gå videre til å se på noen utvalgte konsepter vi mener er viktige å kjenne for å skrive god pythonisk kode.

## TODO

Skrive mer om (?)

- Duck typing
- EAFP vs LBYL
- with statement
- dictionary get, setdefault, og defaultdict
- strengformatering
- key functions
- python moduler og pakker
- script-kode i moduler

        if __name__ == '__main__':
            # script code here


---

Magnus Haug / Kjetil Valle