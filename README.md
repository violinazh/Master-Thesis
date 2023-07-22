LaTeX-Vorlage für Abschlussarbeiten
=======
(English Version below.)

Dies ist die Vorlage für Abschlussarbeiten der Forschungsgruppen Software 
Design and Quality (SDQ) am  KASTEL — Institut für Informationssicherheit 
und Verlässlichkeit des Karlsruher Instituts für Technologie (KIT).

Vielen Dank an Markus Kohm (http://www.komascript.de) für die hilfreiche
Unterstützung beim Erstellen dieser Vorlage.

Version
=======
Version: 1.3.6
Autor: Dr.-Ing. Erik Burger (burger@kit.edu)
mit Beiträgen von Joshua Gleitze

Siehe https://sdq.kastel.kit.edu/wiki/Dokumentvorlagen

Verwendung
==========
Das vorliegende Paket dient als Vorlage für eine Abschlussarbeit. Sie können dazu
die bestehende Hauptdatei `thesis.tex` und die einzelnen Kapiteldateien im
Verzeichnis `sections/` anpassen, indem Sie den Beispieltext entfernen und durch
eigene Inhalte entfernen. Bitte ändern Sie keine Layout-Parameter wie
Schriftgröße, Ränder, Zeilenabstände u.ä. an der Datei, damit die Ausarbeitungen
in einem einheitlichen Format erscheinen.

Die Klasse basiert auf `scrbook` aus dem Paket KOMA-Script. Somit können alle 
Optionen dieser Klasse verwendet werden. 

Optional: Globale Installation
------------------------------
Die Dokumentenklasse kann im texmf-Baum der/des Nutzer:in installiert werden.
Dadurch müssen Dokumente, die die Klasse verwenden, nicht mehr in diesem Ordner liegen.
Hierzu kann das `install`-Skript verwendet werden. Weitere Informationen gibt 
`./install --help`. Je nach System werden root-Rechte zur Installation benötigt.

Sprache
-------
Die Sprache des Dokuments ist standardmäßig auf Englisch eingestellt.
Dies kann in der `\documentclass`-Anweisung am Anfang von `thesis.tex` auf Deutsch 
umgestellt werden.

Einseitig/doppelseitig
----------------------
Das Dokument ist standardmäßig auf doppelseitiges Layout eingestellt, kann aber
durch die Angabe von `oneside` in der `\documentclass`-Anweisung am Anfang von
`thesis.tex` auf einseitiges Layout umgestellt werden.

Draft-Modus
-----------
Der Draft-Modus kann verwendet werden, um eine Entwurfsfassung zu generieren. 
Das kann durch die Option `draft` in der `\documentclass`-Anweisung am Anfang von `thesis.tex` geschehen, oder durch eine Einstellung innerhalb der LaTeX-Umgebung
(z.B. Overleaf: "Compile Mode: Fast (draft)").
Die entsprechende Option für das endgültige Dokument lautet `final`.
Im Draft-Modus werden z.B. todo-Notizen sowie Platzhalter für fehlende Abbildungen angezeigt, im `final`-Modus jedoch ausgeblendet.

LaTeX allgemein
---------------
Siehe https://sdq.kastel.kit.edu/wiki/LaTeX


Verwendung mit [LyX](https://www.lyx.org/WebDe.Home)
====================================================
Diese Klasse hat auch eine Layout-Datei, wodurch sie mit der What-You-See-Is-What-You-Mean-Anwendung [LyX](https://www.lyx.org/WebDe.Home) verwendet werden kann. Hierfür muss erst die Klasse zusammen mit der Layout-Datei installiert werden:
```
./install --lyx
```
Beispieldateien befinden sich im Ordner `lyx/`.


Dateistruktur
============
`thesis.tex`
------------
Dies ist die Hauptdatei des LaTeX-Dokuments. Bitte tragen Sie dort Ihre
Daten ein. Benennen Sie dann die Datei am besten um, damit sie später von
Ihrem Betreuer von anderen leicht unterschieden werden kann
(z.B. in `thesis_erik_burger.tex`).

`thesis.bib`
------------
Dies ist eine BibTeX-Datei, in der Sie Ihre Literatur-Referenzen sammeln
können. Wir empfehlen die Verwendung von biblatex und biber statt BibTeX. 
Dies ist in der Ausarbeitungsvorlage bereits so voreingestellt. Für 
SDQ-relevante Publikationen können Sie die zentralen BibTeX-Dateien einbinden,
siehe https://sdq.kastel.kit.edu/wiki/BibTeX-Literaturlisten

`sdqthesis.cls`
---------------
Dies ist die Vorlage, die die Stil-Informationen für das Dokument enthält.
Im Sinne eines einheitlichen Ausarbeitungsstils soll diese Datei nicht
verändert werden.

`images/`
--------
In diesem Verzeichnis befinden das das SDQ-Logo als PDF und EPS.

`sections/`
-----------
In diesem Verzeichnis können Sie ihre Inhaltsabschnitte als einzelne
`.tex`-Dateien anlegen. Wir empfehlen Ihnen das Aufteilen der Dateien nach
Abschnitten.

`install`
---------
Bash-Skript zur Installation der Klasse unter UNIX.

`sdqthesis.layout`
------------------
Layout-Datei, die die Verwendung der Klasse mit [LyX](https://www.lyx.org/WebDe.Home) ermöglicht.

`lyx/`
------
Enthält Beispieldateien für [LyX](https://www.lyx.org/WebDe.Home), analog zu `thesis.tex` und `sections/*`.

`README.md`
-----------
Dieser Text.

English Version
===============
This is a template for student's final theses at the research groups of Software Design
and Quality (SDQ) at the  KASTEL — Institute of Information Security and Dependability 
at Karlsruhe Institute of Technology (KIT).

Many thanks to Markus Kohm (http://www.komascript.de) for his support in
creating the template.

Version
=======
Version: 1.3.6
Author: Dr.-Ing. Erik Burger (burger@kit.edu)
with contributions by Joshua Gleitze

See https://sdq.kastel.kit.edu/wiki/Dokumentvorlagen

Usage
=====
This package is used as a template for student final theses. To use it, adapt
the main file `thesis.tex` and the files for the chapters in the directory
`sections/` by removing the example text and replacing it with your own content.
Please do not change any layout parameters such as font size, margins, line
spacing etc., so that the theses appear in a uniform way.

The class is based on `scrbook` from the KOMA-Script package. All options of
this class can be used here as well.

Optional: Global installation
-----------------------------
The document class can be installed into the users’ texmf tree. Afterwards, the class
can be used by documents that are not in this folder. You can use the `install` script
to install the class. See `./install --help` for more information. Depending on your 
system, you may require root privileges to install.

Language
--------
The standard language of this document is English. You can change the
language in the `\documentclass` command at the beginning of `thesis.tex`.
German and English are available.

One-sided/two-sided layout
--------------------------
The standard format is two-sided layout. You can change this to one-sided
layout in the `\documentclass` command at the beginning of `thesis.tex`.

Draft mode
----------
The draft mode can be activated with the option `draft`
in the `\documentclass` command at the beginning of `thesis.tex`,
or by choosing the appropriate compile mode in the LaTeX IDE
(e.g., in Overleaf: "Compile Mode: Draft (Fast)")
In `draft` mode, todo-notes and placeholders for missing graphics are displayed,
while they are omitted in `final` mode.

LaTeX
-----
See https://sdq.kastel.kit.edu/wiki/LaTeX


Verwendung mit [LyX](https://www.lyx.org/WebDe.Home)
====================================================
This class also has a layout file, enabling you to use it with the “what you see
is what you mean” editor [LyX](https://www.lyx.org). To do so, you have to first
install the class and the layout file:
```
./install --lyx
```
Example files can be found in the `lyx/` directory.


File structure
==============
`thesis.tex`
------------
This is the main file of your LaTeX document. Please insert your data there.
It is recommended to rename the file so that your advisor can distinguish
different theses (e.g., in `thesis_erik_burger.tex`).

`thesis.bib`
------------
You can use this BibTeX file to collect your literature.
We recommend using biblatex and biber instead of BibTeX.
The template is already configured in this way.
You can include the SDQ literature database for SDQ-relevant publications,
see https://sdq.kastel.kit.edu/wiki/BibTeX-Literaturlisten

`sdqthesis.cls`
---------------
This is the style template for the document. Please do not modify this file,
so that all theses appear in the same style.

`images/`
--------
This directory contains the SDQ logo in PDF and EPS.

`sections/`
-----------
This directory contains your content sections, split in single `.tex` files.
We recommend splitting your sections into single files.

`install`
---------
Bash script to install this class on UNIX.

`sdqthesis.layout`
------------------
Layout file allowing to use the class in [LyX](https://www.lyx.org).

`lyx/`
------
Contains example files for [LyX](https://www.lyx.org), analogous to `thesis.tex` and `sections/*`.

`README.md`
-----------
This text.
