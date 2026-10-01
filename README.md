Festool-Dübelfräse Einweisung
=============================

Einweisung des [FAU FabLab](https://fablab.fau.de) in die Dübelfräse Festool DOMINO DF 500 RQ-Plus.

Inhalt
------

- Regeln und Sicherheit, Betriebsanweisung BA-DF-01 (Aushang bei der Dübelfräse)
- Bedienelemente, Prinzip von Langloch und Dübel, Dübel, Fräser und Frästiefe
- Checkliste, Schutzausrüstung, Material, Absaugung, Werkstück spannen und anzeichnen
- Einstellungen: Frästiefe, Langlochbreite, Höhe, Winkel
- Fräsen Schritt für Schritt, Verleimen, Verbotsliste
- Infos für Betreuer: Fräserwechsel, typische Fehler, Pflege und Prüfung

Download
--------

Die neueste Version aus [GitHub](https://github.com/fau-fablab/festool-duebelfraese-einweisung) ist als PDF abrufbar:

- [Einweisung](https://brain.fablab.fau.de/build/festool-duebelfraese-einweisung/einweisung_Duebelfraese.pdf)
- [Einweisungsliste](https://brain.fablab.fau.de/build/festool-duebelfraese-einweisung/Einweisungsliste_Duebelfraese.pdf)
- [Betriebsanweisung](https://brain.fablab.fau.de/build/festool-duebelfraese-einweisung/Betriebsanweisung_Duebelfraese.pdf) (Aushang bei der Dübelfräse)

Außerdem baut eine GitHub Action die PDFs bei jedem Push. Auf dem Hauptbranch entsteht dabei ein
[Release](https://github.com/fau-fablab/festool-duebelfraese-einweisung/releases) mit Datums-Version (`vJJJJ.MM.TT`) und den PDFs.

Auschecken und bauen
--------------------

```bash
git clone --recursive git@github.com:fau-fablab/festool-duebelfraese-einweisung.git
cd festool-duebelfraese-einweisung
make
```

Die PDFs landen in `output/`. Layout, Kopf- und Fußzeile und das Logo des FAU FabLab (mit
FAU-Schriftzug) kommen aus dem Untermodul [fablab-document](https://github.com/fau-fablab/fablab-document),
das Logo wiederum aus dessen Untermodul [logo](https://github.com/fau-fablab/logo). Bei einem bestehenden
Klon die Untermodule mit `git submodule update --init --recursive` laden.

Technische Details zum Buildserver: [fau-fablab/buildserver](https://github.com/fau-fablab/buildserver)

[![Build Status](https://brain.fablab.fau.de/build/festool-duebelfraese-einweisung/status.svg)](https://brain.fablab.fau.de/build/festool-duebelfraese-einweisung/)
[![PDF bauen](https://github.com/fau-fablab/festool-duebelfraese-einweisung/actions/workflows/pdf.yml/badge.svg)](https://github.com/fau-fablab/festool-duebelfraese-einweisung/actions/workflows/pdf.yml)

Lizenz
------

[![Lizenz: CC BY-SA 3.0](https://licensebuttons.net/l/by-sa/3.0/de/88x31.png)</br>CC BY-SA 3.0](https://creativecommons.org/licenses/by-sa/3.0/)

Die Einweisung und die Betriebsanweisung (`betriebsanweisung/ba_duebelfraese.tex`, BA-DF-01) sind selbst
formuliert und enthalten keine Texte oder Abbildungen aus der Festool-Betriebsanleitung. Alle Zeichnungen
in `zeichnungen/` sind selbst mit TikZ erstellt; Symbole nur nach ISO 7010 aus `fablab-document`.
Die Fotos der Dübelfräse in `bilder/` sind eigene Aufnahmen des FabLabs; das Foto des Langlochs steht unter
CC BY 2.0, siehe [bilder/QUELLEN.md](bilder/QUELLEN.md).
Für Details wird auf die Originalanleitung von Festool verwiesen. **Beim Bearbeiten nichts aus der
Festool-Anleitung übernehmen, auch nicht sinngemäß Satz für Satz.** Bilder bitte selbst zeichnen
oder fotografieren oder nur mit freier, kompatibler Lizenz verwenden.
