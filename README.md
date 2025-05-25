# 📘 Analysis II – Vorlesungsskript in LaTeX

Dies ist ein vollständiges, modular aufgebautes LaTeX-Skript zur **Analysis 2 Vorlesung**.  
Es dokumentiert die Vorlesungsinhalte strukturiert und übersichtlich, mit dem Ziel, später ein passendes **Anki-Karteikarten-Deck** automatisch daraus abzuleiten.

---

## 🔧 Projektstruktur

```mermaid
graph TD
    A[main.tex] --> B[pages/]
    B --> B1[chapter/]
    B1 --> B1a[Kapitel_1-Kurven/]
    B1a --> B1a1[Regularitaet_und_Tangentialvektor.tex]
    B1a --> B1a2[Rektifizierbarkeit_und_Bogenlaenge.tex]
    B1 --> B1b[Kapitel_2-Stetigkeit/]
    B1b --> B1b1[Stetigkeit.tex]
    B1b --> B1b2[Kompaktheit.tex]
    B1b --> B1b3[Zusammenhang.tex]

    A --> C[styling/]
    C --> C1[info-boxen.sty]
    C --> C2[settings.sty]
    C --> C3[prefabs/]
    C3 --> C3a[default-expressions.sty]

    A --> D[img/]
    D --> D1[beispiel.png]
    D --> D2[graph-1.pdf]
```

### Konventionen

- **Kapitelordner:** `Kapitel_1-Kurven`, `Kapitel_2-Stetigkeit` etc.
- **Themendateien:** Keine Leerzeichen oder Umlaute im Dateinamen  
  (`Konvexe_Mengen.tex` statt `Konvexe Mengen.tex`)
- **Struktur:** Jede `.tex` Datei beginnt mit einer `\subsection{...}`

---

## ✨ Features

- 📚 Strukturierung nach Kapitel & Themen
- 🎨 Minimalistisches, druckfreundliches Farbschema (Blau/Grau)
- 📦 Eigene `tcolorbox`-Stile für:
  - Definitionen (hellblau)
  - Sätze, Lemmata, Theoreme (hellgrau)
  - Beispiele, Beweise etc. → neutraler Textfluss
- 🔄 Wiederverwendbare Box-Komponenten (`styling/info-boxen.sty`)
- ⚙️ Kompatibel mit `pgffor` → automatischer Import von Kapitelseiten
- 🧠 Ziel: Grundlage für automatisierte **Anki-Kartengenerierung**

---

## 🚧 In Entwicklung

- [ ] Vollständige Transkription aller Vorlesungsinhalte
- [ ] Automatische Anki-Exportlogik
- [ ] Glossar & Index
- [ ] Mathematische Visualisierungen

---

## 🤝 Mitwirken

Pull Requests mit Korrekturen, Verbesserungen oder Erweiterungen sind jederzeit willkommen.  
Bitte beachte den vorhandenen Stil und die Strukturvorgaben.

