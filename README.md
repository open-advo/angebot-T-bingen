# Angebot: Weiterentwicklung und Pilotierung KIWo 2.0

**Auftraggeber:** Universitätsstadt Tübingen  
**Auftragnehmer:** OpenAdvo UG (haftungsbeschränkt)  
**Angebotsdatum:** 18.05.2026  
**Ansprechpartner:** Leo Reimers · Franz Schwärzler

---

## Zwei Formate

| Format | Einstiegsdatei | Kapitel-Ordner |
|---|---|---|
| **Markdown** | [`angebot.md`](angebot.md) | [`kapitel-md/`](kapitel-md/) |
| **LaTeX** | [`main.tex`](main.tex) | [`kapitel/`](kapitel/) |

---

## Markdown-Version

Kapitel 1 & 2 sind direkt in `angebot.md`. Kapitel 3–7 + Anhang liegen als eigene Dateien in `kapitel-md/`.

**Gesamtdokument zusammenführen:**
```bash
cat angebot.md kapitel-md/*.md > angebot_gesamt.md
```

---

## LaTeX-Version

Kapitel 1 & 2 sind direkt in `main.tex`. Kapitel 3–7 + Anhang liegen in `kapitel/`.

**PDF erzeugen:**
```bash
latexmk -pdf main.tex
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
