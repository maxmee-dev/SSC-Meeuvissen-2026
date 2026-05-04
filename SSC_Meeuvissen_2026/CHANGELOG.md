# SSC — Änderungsprotokoll
### Max Meeuvissen · 4. Mai 2026 · laufend weitergeführt

Dieses Dokument protokolliert alle Änderungen am SSC-Theorierepository in umgekehrter chronologischer Reihenfolge.

**Struktur jedes Eintrags:**
- *Was wurde geändert* — konkrete Dateiänderungen, neue Gleichungen, neue Abschnitte
- *Warum* — kurze Begründung
- *Verweis auf ssc_ergaenzungen.md* — dort steht der theoretische Hintergrund, der Dialog, die Herleitung

**Umgekehrt dazu:** Jeder Eintrag in `ssc_ergaenzungen.md` enthält am Ende einen `→ CHANGELOG`-Verweis auf den zugehörigen Commit hier.

### Versionsschema

| Version | Bedeutung |
|---------|-----------|
| 0.x.0 | Neue Theorieinhalte (neue Einträge, neue Gleichungen, konzeptuelle Erweiterungen) |
| 0.x.y | Dokumentupdates, Korrekturen, Formatierung ohne neue Theorie |

---

## v0.9.0 · `[aktuell]` · 4. Mai 2026 · nach 22:27

**Art:** Changelog erstellt, Versionsnummern eingeführt, PDF mit Seitenzahlen + Timestamp + Version

### CHANGELOG.md erstellt (diese Datei)
Vollständige rückwirkende Dokumentation aller Commits. Bidirektionale Referenzierung mit `ssc_ergaenzungen.md`.

### Versionsnummern ins System eingeführt
PDF-Header, HTML-Titelseite und Footer tragen ab jetzt Versionsnummer + Timestamp.

### PDF: Seitenzahlen + Timestamp + Versionsnummer
`pdf_gesamt.pdf` enthält jetzt Seitenzahlen (unten rechts) und Versionsstempel (unten links) auf jeder Seite.

---

## v0.8.0 · `efae375` · 4. Mai 2026 · 22:27

**Art:** Vollständige Aktualisierung aller Hauptdateien + PDF-Neugenerierung

### Tagline in alle Dokumente eingefügt
> „Einstein sagte, Raum und Zeit sind relativ. Ich sage, Raumzeit selbst ist bedingt — sie existiert nicht überall. Und das löst den Widerspruch zwischen Relativitätstheorie und Quantenmechanik."

Eingefügt in: `README.md`, `ssc_ergaenzungen.md`, `ssc_mathematik.md`, `ssc_gesamt.html` (als Zitatblock nach Titelseite), `ssc_paper.tex` (als Epigraph nach Titelseite).

### J(T)-Korrektur in ssc_paper.tex und ssc_gesamt.html
Der bisherige Quellterm J(T) = κ·T/(T+T₀) war ein positiver Treiber — hohe Energiedichte erzeugt Raumzeit. Das ist kausal inkonsistent: T existiert nur wo Φ > 0, also kann T nicht die Ursache von Φ sein.

Neuer Ansatz: J(T) = −κ · max(0, T − T_c) / T_c — destruktiver Term. T zerstört Raumzeit oberhalb der Schwelle T_c, es erzeugt sie nicht.

→ **Theoretischer Hintergrund:** `ssc_ergaenzungen.md`, Eintrag 012

### Autonome Expansionsfront ergänzt
Da die Expansionsfront nicht durch Materie angetrieben wird, gilt:

□Φ + V′(Φ) = 0

Topologisch stabile Domänenwand im Doppeltopf-Potential. In `ssc_paper.tex` als Gl. (eq:autonomous), in `ssc_gesamt.html` als Gl. (8b).

→ **Theoretischer Hintergrund:** `ssc_ergaenzungen.md`, Eintrag 012

### Dunkle Energie — mathematische Konsequenz dokumentiert
Grenzflächenspannung σ → ρ = 3σ/R → w ≈ −1/3. Beobachtet: w ≈ −1. Diskrepanz offen.

In `ssc_gesamt.html` (Sektion 5), in `ssc_paper.tex` (Open Problem 5), in `ssc_ergaenzungen.md` (Abschnitt 3.3).

→ **Theoretischer Hintergrund:** `ssc_ergaenzungen.md`, Eintrag 013

### Open Problem 7 ergänzt (fehlend)
Das fehlende Problem 7 im LaTeX-Paper nachgetragen: konzeptuelle Frage zum Blasen-Multiversum.

### Neue Open Problems 13–14 in ssc_paper.tex
- Problem 13: Ist Expansion passiv, aktiv oder bidirektional?
- Problem 14: Welcher Mechanismus liefert w = −1 statt w = −1/3?

→ **Theoretischer Hintergrund:** `ssc_ergaenzungen.md`, Eintrag 013

### Offene Fragen 12–14 in ssc_gesamt.html
Entsprechende neue Fragen in Sektion 17 (Offene Fragen) der HTML ergänzt.

### PDF neu generiert
`pdf_gesamt.pdf` — 102 KB — mit allen obigen Änderungen.

---

## v0.7.0 · `f87758d` · 4. Mai 2026 · 21:56

**Art:** Neue Einträge 012 und 013 in ssc_ergaenzungen.md + Korrekturen offene Fragen

### Eintrag 012 — Φ misst nur Raumzeit-Präsenz
Präzisierung: Φ beschreibt ausschließlich das Vorhandensein von Raumzeit, nicht ihren Inhalt. Konsequenz: J(T) kann kein positiver Quellterm sein (→ Reformulierung, s.o.).

→ **Vollständige Dokumentation:** `ssc_ergaenzungen.md`, Eintrag 012

### Eintrag 013 — Bidirektionaler Expansionsmechanismus
Spekulativer Ansatz: Raumzeit breitet sich aktiv aus UND der Superzustand zieht gleichzeitig an. Mathematische Analyse zeigt w ≈ −1/3 statt −1. Konzeptuelle Spannung (Superzustand ohne Raumzeitstruktur, der dennoch „zieht") offen benannt.

→ **Vollständige Dokumentation:** `ssc_ergaenzungen.md`, Eintrag 013

### Offene Fragen bereinigt
- Duplikate (Fragen 8/9 = Kopien von 5/6) als solche markiert und aus der Nummerierung entfernt
- Umnummerierung 10–14 → 8–12
- Neue Fragen 13–15 eingefügt

---

## v0.6.1 · `5bbc6a4` · 4. Mai 2026 · 21:34

**Art:** Repository-Struktur bereinigt

### Veraltete Dateien in archiv/ verschoben
Folgende Dateien sind durch `ssc_gesamt.html` + `ssc_paper.tex` überholt und wurden in `archiv/` verschoben (nicht gelöscht — historischer Wert erhalten):

`ssc_diskussion.html`, `ssc_erklaerung_de.html`, `ssc_simple.html`, `pdf_desktop.pdf`, `pdf_diskussion.pdf`, `pdf_druck.pdf`, `pdf_mobile.pdf`, `pdf_simple.pdf`, `LIES_MICH.txt`

Neue Hauptdokumente: `ssc_gesamt.html` / `pdf_gesamt.pdf` (deutsch, vollständig), `ssc_paper.tex` (englisches Preprint).

---

## v0.6.0 · `35dee86` · 4. Mai 2026 · 17:58

**Art:** Neues Gesamtdokument erstellt

### ssc_gesamt.html + pdf_gesamt.pdf (44 KB HTML / 95 KB PDF)
Vollständiges deutsches Theoriepapier mit 17 Sektionen, CSS-Formatierung, Status-Markierungen (Established / Candidate / Open), allen Gleichungen in HTML, Inhaltsverzeichnis. Ersetzt alle bisherigen HTML-Versionen als kanonisches Deutschdokument.

→ Inhalt: alle Einträge 001–011 aus `ssc_ergaenzungen.md`

---

## v0.5.1 · `059b850` · 4. Mai 2026 · 17:46

**Art:** LaTeX-Paper vollständig auf aktuellen Stand gebracht

### ssc_paper.tex auf Stand Einträge 001–011
Alle Theorieinhalte bis Eintrag 011 in das LaTeX-Preprint übertragen:
- Sektion 2.4: Zwei Dimensionen von Φ
- Sektion 2.5: Zwei Modelle für Superzustand ↔ Superposition
- Sektion 2.6: Warum Messung die Position fixiert
- Sektion 6: Was ist genuinely new (8 Punkte, inkl. QM+GR-Vereinigung)
- Sektion 8 (Open Problems) auf 12 Probleme erweitert

→ **Theoretischer Hintergrund:** `ssc_ergaenzungen.md`, Einträge 001–011

---

## v0.5.0 · `27151c1` · 4. Mai 2026 · 17:41

**Art:** Mathematisches Framework als neue Sektion 7 in ssc_paper.tex

### Sektion 7 — Mathematische Formalisierung
Erste vollständige mathematische Formalisierung im LaTeX-Preprint:
- Definition 1: Φ als Skalarfeld
- Definition 2: Komplementarität Φ + Ψ = 1
- Gl. (4): Erweiterte Feldgleichung Φ·G_μν = 8π·T_μν
- Gl. (5): Bianchi-Konsequenz
- Gl. (6–8): Φ-Dynamikgleichung mit Potential und Quellterm
- Kosmologische Randbedingung
- Φ-modifizierte Klein-Gordon-Gleichung
- Statustabelle (Established / Candidate / Open)

→ **Mathematischer Hintergrund:** `ssc_mathematik.md`, Sitzungen 1–2

---

## v0.4.0 · `0817228` · 4. Mai 2026 · 16:33

**Art:** Neue Einträge 008–011 in ssc_ergaenzungen.md

### Eintrag 008 — Zwei Dimensionen von Φ
Φ misst zwei physikalisch verschiedene Dinge: (1) ob Teilchen als definierte Objekte existieren (nur Φ = 0 / Φ > 0), (2) ob Positionen definiert sind (Φ = 1 vs. 0 < Φ < 1). Klare Unterscheidung Superzustand ↔ Quantensuperposition.

### Eintrag 009 — Superposition als universelle Grundstruktur
Superposition ist kein Laborphänomen. Jedes Atom enthält Superposition auf Ebene von Elektronen und Quarks — Überrest des Superzustands in aller Materie.

### Eintrag 010 — Zwei Modelle Superzustand ↔ Superposition
Modell A (Einwirkung) vs. Modell B (Transformation). Modell B konsistenter mit SSC-Ausschlussprinzip — bevorzugt.

### Eintrag 011 — Vereinigung QM + GR als 10. adressiertes Problem
GR = Φ = 1-Grenzfall, QM = 0 < Φ < 1-Regime. Kein echter Widerspruch — verschiedene Bereiche desselben Spektrums.

→ **Vollständige Dokumentation:** `ssc_ergaenzungen.md`, Einträge 008–011

---

## v0.3.1 · `6a3923f` · 4. Mai 2026 · 16:00

**Art:** Sitzung 2 in ssc_mathematik.md

### Zwei-Ebenen-Struktur von Φ
Henne-Ei-Problem gelöst: ρ setzt Raumzeit voraus, kann also nicht Ursache von Φ sein. Lösung: zwei Ebenen — kosmologisch (Expansionsfront bestimmt Φ global) vs. lokal (physikalische Abweichungen innerhalb der Raumzeit). Kosmologische Randbedingung R(t) = ∫c·a(t')dt' hergeleitet.

→ **Vollständige Dokumentation:** `ssc_mathematik.md`, Sitzung 2

---

## v0.3.0 · `7cf0f04` · 4. Mai 2026 · 15:32

**Art:** Sitzung 1 in ssc_mathematik.md

### Erste mathematische Formulierung
Φ als Skalarfeld Φ(x, t) mit 0 ≤ Φ ≤ 1. Erster Ansatz Φ(ρ) = ρ/(ρ + ρ₀). Sofort als Kandidat eingestuft, nicht als bewiesene Gleichung.

→ **Vollständige Dokumentation:** `ssc_mathematik.md`, Sitzung 1

---

## v0.2.0 · `6cc182a` · 4. Mai 2026 · 12:11

**Art:** Eintrag 007 in ssc_ergaenzungen.md

### Eintrag 007 — Warum Messung die Position fixiert
Das Messgerät ist kein privilegierter Akteur. Es ist einfach das erste massive Objekt mit vollständig ausgebildeter Raumzeit, das das Teilchen berührt. Jede Wechselwirkung mit Φ ≈ 1 ist eine Messung. Der Beobachter ist nicht besonders.

→ **Vollständige Dokumentation:** `ssc_ergaenzungen.md`, Eintrag 007

---

## v0.1.0 · `cefabf7` · 4. Mai 2026 · 12:04

**Art:** Initial Commit

### Theorie vollständig erstentwickelt (Einträge 001–006)
SSC-Theorie in einem einzigen Gespräch entstanden. Kerninhalte: prä-raumzeitlicher Superzustand, SSC-Prinzip, Expansion als Wellenfront, Singularität als Phasenübergang, Informationsparadoxon, zyklische Kosmologie. 9 adressierte Probleme der Physik. Erste Korrekturen (Urknall-Formulierung) bereits eingearbeitet.

Dateien: `ssc_paper.tex`, `ssc_references.bib`, `ssc_ergaenzungen.md`, `ssc_erklaerung_de.html`, `ssc_simple.html`

→ **Vollständige Dokumentation:** `ssc_ergaenzungen.md`, Einträge 001–006
