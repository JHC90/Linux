# Basic Interaktion

## Erstellen
>touch Test.txt

hiermit wird eine Leere Datei angelegt. Es muss kein Dateityp hinterlegt sein

## Betrachten mit cat
> cat Test.txt

hiermit kann eine Datei unmittelbar auf der Kommandozeile betrachtet werden. Ist natürlich witzlos bei einer leeren Datei

## Betrachten der ersten bzw letzten zeile

**Head**
> head Test.txt

zeig die ersten 10 Zeilen von Test.txt

> head -n 5 Test.txt

Zeigt diersten 5 Zeilen

Head ist v.a. dann interessant wenn die wichtigen Informationen in den ersten Zeilen Liegen. Bspw bei einer Raw-Format einer Email


**Tail**
gleich wie Head nur mit Tail


> tail -5 Test.txt

Tail ist vorallem bei der Auswertung von Log-Dateien interessant


## More

> more Test.txt

Hiermit wir ein Programm geöffnet mit welchem man via Enter durch die Datei ausschließlich vorwärt blättern kann. mit strg +C kann man das Programm schließen

## Less
less ist ein erweitertes Programm von more, mit diesem Programm kann man mit den Pfeiltasten durch die Datei vor und zurückblättern