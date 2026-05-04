# SSC — Mathematische Grundlegung
### Max Meeuvissen · Beginn: 4. Mai 2026

Dieses Dokument protokolliert die schrittweise mathematische Formalisierung der SSC-Theorie.  
Es entsteht im Dialog: Max beschreibt seine Intuition, Claude übersetzt sie in Mathematik.

**Jede Gleichung wird erklärt. Jede Unsicherheit wird benannt. Nichts wird gelöscht.**

---

## ◆ ANWEISUNGEN FÜR CLAUDE

- Immer eine Frage auf einmal stellen — nie mehrere gleichzeitig
- Jede Gleichung in Alltagssprache erklären, direkt danach
- Physikalische oder mathematische Probleme sofort benennen, nicht beschönigen
- Den Arbeitsprozess vollständig dokumentieren: Fragen, Antworten, Gleichungen, Korrekturen
- Neue Sitzungen als eigene Abschnitte kennzeichnen

---

## Ausgangspunkt

**Kernthese, die formalisiert werden soll:**

> Raumzeit und Superzustand sind komplementäre, sich gegenseitig ausschließende Zustände eines fundamentalen Substrats.

**Der Ordnungsparameter Φ:**

| Wert | Bedeutung |
|------|-----------|
| Φ = 1 | Vollständige Raumzeit |
| Φ = 0 | Vollständiger Superzustand |
| 0 < Φ < 1 | Übergangsbereich (z.B. Quantenebene) |

Ziel dieser Formalisierung: Die Dynamik von Φ beschreiben — also wie und warum er sich verändert.  
Alles andere (Expansion, Schwarze Löcher, Kollaps) folgt später als Konsequenz.

---

## Sitzung 1 — 4. Mai 2026

### Klärung vorab (aus separater Sitzung)

**Max:** Φ beschreibt den Zustand eines Bereichs im Substrat — nicht global, sondern lokal. Die Grenze zwischen Φ = 1 und Φ = 0 ist die kosmische Expansionsfront. Sie ist durch bekannte Größen definiert:

- Alter des Universums: 13,8 Milliarden Jahre
- Radius des beobachtbaren Universums: ~46 Milliarden Lichtjahre
- Die Expansionsfront bewegt sich mit der gemessenen Expansionsgeschwindigkeit — das ist dieselbe Größe, keine zusätzliche Annahme

Innerhalb der Front: Φ = 1 (Raumzeit — Ort, Zeit, Masse, Kausalität)  
Außerhalb der Front: Φ = 0 (Superzustand)

**Offene Frage:** Ist der Übergang an der Front scharf (Φ springt von 1 auf 0) oder fließend (Φ durchläuft einen Gradienten)?

---

### Frage 1 an Max:

**Claude:** Ist der Übergang an der Expansionsfront scharf oder fließend — und gibt es in deiner Theorie einen Grund, warum er das eine oder das andere sein müsste?

**Max:** Was sagt die aktuelle Wissenschaft dazu? Und wir müssen erklären, warum Superposition auf Quantenebene (als Überbleibsel des Superzustands) weiter besteht.

**Auswertung:**

Die Standardkosmologie stellt diese Frage nicht — das FLRW-Modell hat keine physikalische Grenze. SSC betritt hier Neuland.

Die Antwort auf scharf/fließend ergibt sich aus der Theorie selbst: Wenn der Übergang scharf wäre, wäre Φ = 1 überall innerhalb des Universums — ohne Ausnahme. Dann gäbe es keinen Grund, warum auf Quantenebene Superposition erhalten bleibt. Also muss gelten:

> **Der Übergang ist fließend — und Φ ist kein globaler Schalter, sondern ein Feld, das von der lokalen Masse-Energie-Dichte abhängt.**

| Bereich | Energie-Dichte | Φ | Superposition |
|---------|---------------|---|---------------|
| Kosmische Grenze | → 0 | → 0 | total |
| Quantenebene | sehr klein | knapp unter 1 | partiell erhalten |
| Makroobjekte | groß | ≈ 1 | unterdrückt |
| Schwarzes Loch (Singularität) | → ∞ | → 0 (Phasenübergang) | total |

Das verbindet drei Beobachtungen mit einem einzigen Mechanismus:
1. Quantensuperposition existiert — weil Φ auf Quantenebene < 1
2. Decoherence nimmt mit Masse zu — weil mehr Masse → Φ → 1
3. Die Expansionsfront ist ein Gradient, keine Membran

---

### Erste mathematische Formulierung

**Φ als Feld:**

Φ ist keine Konstante und kein globaler Schalter — es ist ein **Skalarfeld**: jedem Punkt im Raum wird ein Wert zwischen 0 und 1 zugewiesen.

$$\Phi = \Phi(\mathbf{x}, t) \quad \text{mit} \quad 0 \leq \Phi \leq 1$$

*In Worten: Φ hat an jedem Ort x und zu jeder Zeit t einen eigenen Wert.*

**Φ hängt von der lokalen Masse-Energie-Dichte ab:**

Die einfachste mathematische Beziehung, die das ausdrückt:

$$\Phi(\rho) = \frac{\rho}{\rho + \rho_0}$$

*In Worten: Je größer die lokale Energiedichte ρ (rho), desto näher an 1 ist Φ. Bei ρ = 0 (kein Inhalt, Superzustand) ist Φ = 0. Bei sehr großem ρ geht Φ gegen 1.*

**Was ist ρ₀?** Eine charakteristische Energiedichte — der Schwellenwert, bei dem Φ = 0,5 ist, also genau auf der Hälfte zwischen Superzustand und vollständiger Raumzeit. Ihr Wert ist noch offen. `[?]`

**⚠ Ehrliche Einschränkung:** Diese Formel ist ein erster Ansatz — sie beschreibt die richtige Grundstruktur (Φ steigt mit ρ, geht von 0 nach 1), aber sie ist noch nicht aus tieferen Prinzipien hergeleitet. Sie ist ein Kandidat, keine bewiesene Gleichung.

---

### Nächste offene Frage für Sitzung 2:

Was bestimmt ρ₀? Ist es die Planck-Dichte, eine kosmologische Größe, oder etwas anderes? Und wie beschreiben wir die Dynamik — also wie verändert sich Φ über Zeit und Raum?

---
