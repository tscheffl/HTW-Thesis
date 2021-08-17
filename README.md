# HTW-Thesis
LaTeX Template für Abschlussarbeiten im Studiengang IKT der [HTW-Berlin](https://ikt-bachelor.htw-berlin.de/)

##Notwendige Anpassungen in der Vorlage

Die Vorlage ist für die Erstellung von Arbeiten in deutscher und englischer Sprache geeignet. Die Umstellung der Sprache erfolgt in der Datei `settings/adjustments.tex`


In der Hauptdatei `Thesis.tex` müssen die allgemeinen Angaben zum Author und Titel, usw. in die passenden Felder eingetragen werden. Die einzelnen Kapitel werden dann per `/input{}` importiert.

##Erstellung des PDF-Dokuments

Um die Verzeichnisse (Literatur, Abkürzungen und Index) zu erstellen sind folgende Befehle und ein weiterer LaTeX Lauf notwendig:
  
  *   `biber Thesis`
  *   `makeindex Thesis.nlo -s nomencl.ist -o Thesis.nls`
  *   `makeindex Thesis`
  
  
**Hinweis:** Alternativ kann für die Erstellung des Literaturverzeichnis statt `biber` auch `bibtex` verwendet werden. Dazu muss in der Datei `settings/adjustments.tex` im Bereich Literaturverarbeitung das passende Kommando ausgewählt werden.

##Kontakt:

Probleme und Ergänzungsvorschläge bitte per Email an [thomas.scheffler@htw-berlin.de](mailto:thomas.scheffler@htw-berlin.de?subject=Github:%20HTW-LaTeX-Vorlage) melden.
