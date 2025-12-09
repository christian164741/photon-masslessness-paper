Vorlage-paper/
```
├── bib/                     # Zentrale BibLaTeX-Datenbank
│   └── literatur.bib
│
├── de/                      # Deutsche Version
│   ├── main.tex             # Hauptdatei (Deutsch)
│   ├── captures/            # Kapitel / Abschnitte
│   └── figures/             # Abbildungen
│
├── en/                      # English version
│   ├── compton_en.tex       # Main file (English)
│   ├── captures/
│   └── figures/
│
└── styles/                  # Styles & Makros für Paper
    ├── paper-style-de.sty
    └── paper-style-en.sty

```

## 📖 Kompilieren

### 1. Deutsche Version
```
cd de
pdflatex main_en.tex


```
### 2. Englische Version
```
cd en
main_en.tex
```

👉 In **TeXstudio** reicht es, `main_en.tex` zu kompilieren, wenn folgende Einstellungen aktiv sind:
- Bibliographie-Tool: **Biber**
- Index-Tool: **MakeIndex** oder **Xindy** (empfohlen für Umlaute)
- "Erzeugen & Ansicht" → Standard: `pdflatex → biber → makeindex → pdflatex ×2`

## 📚 Literatur
```
bib/literatur.bib


```
## 🔤 Index

```
\printindex[myindex]

```


## 🗂️ GitHub-Hinweise

- Temporäre LaTeX-Dateien (aux, log, bbl, blg, toc, pdf …) sind in `.gitignore`.
- Im Repo liegen nur die **Quellen** (Tex, Bib, Bilder, Styles).
- PDFs werden lokal erzeugt, nicht im Repo gespeichert.

---

✍️ **Autor:** Christian Weilharter, Dipl.-Ing. (FH)  
📅 Stand: Oktober 2025

- 🌐 Website: [https://mathandphysics.de](https://mathandphysics.de)
