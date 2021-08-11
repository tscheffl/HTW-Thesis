# HTW-Thesis
LaTeX Template für Abschlussarbeiten im Studiengang IKT der HTW-Berlin.de

Die Vorlage ist für die Erstellung von Arbeiten in deutscher und englischer Sprache geeignet. Die Umstellung der Sprache erfolgt in der Datei `settings/adjustments.tex`

In der Hauptdatei `thesis.tex` müssen die allgemeinen Angaben zum Author und Titel, usw. in die passenden Felder eingetragen werden. Die einzelnen Kapitel werden dann per `/include{}` importiert.

Um die Verzeichnisse (Literatur, Abkürzungen und Index) zu erstellen sind folgende Befehle und ein weiterer LaTeX Lauf notwendig:
  
  *   `biber Thesis`
  *   `makeindex Thesis.nlo -s nomencl.ist -o Thesis.nls`
  *   `makeindex Thesis`
  
  
Probleme und Ergänzungsvorschläge bitte per Email an [thomas.scheffler@htw-berlin.de](mailto:thomas.scheffler@htw-berlin.de?subject=Github:%20HTW-LaTeX-Vorlage) melden.
