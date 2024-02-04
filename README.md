# HTW-Thesis
LaTeX Template für Abschlussarbeiten im Studiengang IKT der [HTW-Berlin](https://ikt-bachelor.htw-berlin.de/)

## Notwendige Anpassungen in der Vorlage

Die Vorlage ist für die Erstellung von Arbeiten in deutscher und englischer Sprache geeignet. Die Umstellung der Sprache erfolgt in der Datei `settings/adjustments.tex`


In der Hauptdatei `Thesis.tex` müssen die allgemeinen Angaben zum Author und Titel, usw. in die passenden Felder eingetragen werden. Die einzelnen Kapitel werden dann per `/input{}` importiert.

Eigene Packages können hier vor dem Abschnitt `\begin{document}` eingefügt werden.


## Verwendung von Anführungszeichen in deutschen Texten

In LaTeX ist es leider nicht einfach Anführungszeichen für deutsche Texte zu verwenden. Es müssen spezielle Packages oder Befehle verwendet werden. Die einfache Eingabe von `".." ` führt in der Regel zu unvorhergesehenen Ergebnissen.

Diese Vorlage verwendet das Package [csquotes](https://ctan.org/pkg/csquotes?lang=de). Normaler Text lässt sich mit dem Befehl `\enquote{Text in Anführungszeichen}` in Anführungszeichen setzen.
Zitate können z.B. mit `\blockquote{}` vom restlichen Text abgesetzt werden.
Ich empfehle immer zu prüfen, ob Anführungszeichen wirklich notwendig sind. Um bestimmte Begriffe optisch hervorzuheben, sollten Sie besser `\emph{}` verwenden.

## Erstellung des PDF-Dokuments

Um die Verzeichnisse (Literatur, Abkürzungen und Index) zu erstellen sind folgende Befehle und ein weiterer LaTeX Lauf notwendig:
  
  *   `biber Thesis`
  *   `makeindex Thesis.nlo -s nomencl.ist -o Thesis.nls`
  *   `makeindex Thesis`
  
  
**Hinweis:** Alternativ kann für die Erstellung des Literaturverzeichnis statt `biber` auch `bibtex` verwendet werden. Dazu muss in der Datei `settings/adjustments.tex` im Bereich Literaturverarbeitung das passende Kommando ausgewählt werden.

## Kontakt:

Probleme und Ergänzungsvorschläge bitte per Email an [thomas.scheffler@htw-berlin.de](mailto:thomas.scheffler@htw-berlin.de?subject=Github:%20HTW-LaTeX-Vorlage) melden.
