# Angebot: Weiterentwicklung und Pilotierung KIWo 2.0

**Auftraggeber:** Universitätsstadt Tübingen  
**Auftragnehmer:** OpenAdvo UG (haftungsbeschränkt)  
**Angebotsdatum:** 15.05.2026  
**Ansprechpartner:** Leo Reimers · Franz Schwärzler

---

## Zwei Formate

| Format | Einstiegsdatei | Kapitel-Ordner |
|---|---|---|
| **Markdown** | [`angebot.md`](angebot.md) | [`kapitel-md/`](kapitel-md/) |
| **LaTeX** | [`main.tex`](main.tex) | [`kapitel/`](kapitel/) |

---

## Markdown-Version

Kapitel 1 & 2 sind direkt in `angebot.md`. Kapitel 3–13 liegen als eigene Dateien in `kapitel-md/` und sind per Link verknüpft.

**Gesamtdokument zusammenführen:**
```bash
cat angebot.md kapitel-md/*.md > angebot_gesamt.md
```

**Platzhalter finden:**
```bash
grep -rn "\[" kapitel-md/ angebot.md
```

---

## LaTeX-Version

Kapitel 1 & 2 sind direkt in `main.tex`. Kapitel 3–13 liegen in `kapitel/` und werden per `\input{}` eingebunden.

**PDF erzeugen:**
```bash
latexmk -pdf main.tex
# oder
pdflatex main.tex && pdflatex main.tex
```

**Platzhalter finden:**
```bash
grep -rn "\\\\ph{" kapitel/ main.tex
```

**Aufräumen:**
```bash
latexmk -c
```

---

## Kontakt

| Name | E-Mail |
|---|---|
| Leo Reimers | leo.reimers@openadvo.com |
| Franz Schwärzler | franz.schwaerzler@openadvo.com |
