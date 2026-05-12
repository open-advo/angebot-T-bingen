# Angebot: Weiterentwicklung und Pilotierung KIWo 2.0

**Auftraggeber:** Universitätsstadt Tübingen  
**Auftragnehmer:** OpenAdvo UG (haftungsbeschränkt)  
**Angebotsdatum:** 15.05.2026  
**Ansprechpartner:** Leo Reimers · Franz Schwärzler

---

## Inhalt

Das Dokument `main.tex` enthält die vollständige Angebotsvorlage mit
drei Paketvarianten (Basis / Empfohlen / Vollausbau) und folgendem Aufbau:

| Kapitel | Inhalt |
|---------|--------|
| 1 | Anschreiben |
| 2 | Management Summary |
| 3 | Paketvergleich |
| 4 | Ausgangslage und Anschluss an KIWo |
| 5 | Zielbild und Scope der Weiterentwicklung |
| 6 | Leistungsbeschreibung je Paket |
| 7 | Vorgehen und Projektplan |
| 8 | Projektorganisation |
| 9 | Technische und betriebliche Rahmenbedingungen |
| 10 | Preisangebot |
| 11 | Vertragliche Rahmenbedingungen |
| 12 | Über OpenAdvo |
| 13 | Anlagen |

---

## Platzhalter ausfüllen

Alle noch zu befüllenden Stellen sind im Quelltext als
`\ph{...}` markiert und erscheinen im PDF in grauer Kursivschrift.
Einfach suchen und ersetzen:

```
grep -n "\\\\ph{" main.tex
```

---

## PDF erzeugen

### Einmalig (pdflatex)

```bash
pdflatex -interaction=nonstopmode main.tex
pdflatex -interaction=nonstopmode main.tex   # zweimal für Inhaltsverzeichnis
```

### Mit latexmk (empfohlen)

```bash
latexmk -pdf main.tex
```

Zum Aufräumen:

```bash
latexmk -c
```

### Benötigte LaTeX-Pakete

Das Dokument nutzt Standard-CTAN-Pakete. Bei einer vollständigen
TeX-Live- oder MiKTeX-Installation sind alle Pakete vorhanden:

`lmodern` · `microtype` · `parskip` · `geometry` · `booktabs` ·
`longtable` · `tabularx` · `xcolor` · `colortbl` · `amssymb` ·
`pifont` · `hyperref` · `fancyhdr` · `titlesec`

---

## Kontakt

| Name | E-Mail |
|------|--------|
| Leo Reimers | leo.reimers@openadvo.com |
| Franz Schwärzler | franz.schwaerzler@openadvo.com |
