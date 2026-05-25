# AI-assisted Requirements & User Stories Generator

## Projektbeschreibung

In diesem Projekt wird untersucht, wie gut KI-Tools wie ChatGPT und Gemini dabei helfen können, aus einfachen Softwareideen strukturierte Requirements und User Stories zu erstellen.

Der Fokus liegt nicht auf der Entwicklung einer fertigen Software, sondern auf einem dokumentierten Workflow im Bereich Requirements Engineering. Dabei wird getestet, ob KI besonders Personen ohne viel Programmier- oder Software-Engineering-Erfahrung unterstützen kann, wichtige Anforderungen, User Stories, Akzeptanzkriterien und mögliche Sonderfälle besser zu erkennen.

Das Projekt wurde im Rahmen eines Kurses zu AI-assisted Software Engineering erstellt.

## Ziel des Projekts

Das Ziel des Projekts ist es herauszufinden, ob KI-generierte Requirements und User Stories hilfreich, verständlich und vollständig genug sind, um eine Softwareidee besser zu strukturieren.

Dabei stehen folgende Fragen im Mittelpunkt:

- Erkennt KI wichtige Funktionen einer Anwendung?
- Ergänzt KI sinnvolle Anforderungen, an die Anfänger eventuell nicht denken würden?
- Sind die Ergebnisse verständlich und gut strukturiert?
- Welche Unterschiede gibt es zwischen ChatGPT und Gemini?
- Welche Prompt-Strategie liefert die besten Ergebnisse?
- Wo liegen die Grenzen der KI-Ergebnisse?

## Untersuchte Anwendungsideen

Im Projekt wurden zwei Anwendungsideen mit unterschiedlicher Komplexität betrachtet:

| Anwendungsidee | Komplexität | Beschreibung |
|---|---|---|
| Simple To-do List | niedrig | Eine einfache App zum Erstellen, Bearbeiten, Löschen und Abhaken von Aufgaben |
| Student Task Manager | mittel | Eine App zur Verwaltung von Aufgaben, Deadlines, Kursen und Lernfortschritt |

Für beide Anwendungsideen wurde zuerst eine manuelle Baseline erstellt. Danach wurden mit ChatGPT und Gemini Requirements und User Stories generiert und anschließend verglichen.

## Vorgehensweise

Das Projekt wurde in mehreren Schritten durchgeführt:

1. Anwendungsideen mit unterschiedlicher Komplexität auswählen
2. Manuelle Baseline für Requirements und User Stories erstellen
3. Prompt-Templates und Prompt-Strategien definieren
4. Requirements und User Stories mit ChatGPT und Gemini generieren
5. KI-Ergebnisse mit der Baseline vergleichen
6. Metriken und Chatverläufe dokumentieren
7. Strukturierte Selbstevaluierung durchführen
8. Ergebnisse auswerten und README schreiben
9. Präsentation vorbereiten

Diese Vorgehensweise orientiert sich am geplanten Workflow aus dem Projektvorschlag.

## Verwendete KI-Tools

Im Projekt wurden folgende KI-Systeme verwendet:

- ChatGPT
- Gemini

Beide Tools wurden mit denselben oder sehr ähnlichen Prompts getestet, damit die Ergebnisse besser vergleichbar sind.

## Prompt-Strategien

Es wurden drei verschiedene Prompt-Arten verwendet:

### 1. Simple Prompt

Beim Simple Prompt wurde nur eine kurze und allgemeine Aufgabenbeschreibung eingegeben.

Beispiel:

```text
Erstelle Requirements und User Stories für eine einfache To-do-Listen-App.
```

Der Simple Prompt sollte zeigen, welche Ergebnisse entstehen, wenn die KI nur sehr wenig Vorgaben erhält.

### 2. Structured Prompt

Beim Structured Prompt wurden der KI klare Vorgaben gemacht. Zum Beispiel sollte sie funktionale Requirements, nicht-funktionale Requirements und User Stories in einer übersichtlichen Struktur erstellen.

Beispiel:

```text
Erstelle Requirements und User Stories für eine einfache To-do-Listen-App.

Berücksichtige dabei:
- funktionale Requirements
- nicht-funktionale Requirements
- User Stories im Format: Als Benutzer möchte ich ..., damit ...
- eine klare und übersichtliche Struktur
```

Diese Prompt-Art führte zu besser gegliederten Ergebnissen, weil die KI genauer wusste, welche Inhalte erwartet werden.

### 3. Iterative Prompt

Beim Iterative Prompt wurde das Ergebnis schrittweise verbessert. Zuerst wurde ein einfaches Ergebnis erzeugt, danach wurden fehlende funktionale und nicht-funktionale Requirements ergänzt und anschließend die User Stories überarbeitet.

Beispiel:

```text
Prompt 1:
Erstelle Requirements und User Stories für eine einfache To-do-Listen-App.

Prompt 2:
Überarbeite das Ergebnis und ergänze fehlende funktionale und nicht-funktionale Requirements.

Prompt 3:
Verbessere die User Stories und achte darauf, dass sie im Format „Als Benutzer möchte ich ..., damit ...“ geschrieben sind.
```

Der iterative Prompt sollte zeigen, ob ein schrittweises Vorgehen zu besseren und vollständigeren Ergebnissen führt.

## Repository-Struktur

Die Projektdateien sind in mehrere Ordner aufgeteilt, damit Baselines, Prompts, KI-Ergebnisse, Vergleiche, Evaluation und Präsentationsmaterialien übersichtlich getrennt sind.

```text
.
├── ai-results
│   ├── chatgpt
│   │   ├── student-task-manager-iterative.md
│   │   ├── student-task-manager-simple.md
│   │   ├── student-task-manager-structured.md
│   │   ├── todo-list-iterative.md
│   │   ├── todo-list-simple.md
│   │   └── todo-list-structured.md
│   └── gemini
│       ├── student-task-manager-iterative.md
│       ├── student-task-manager-simple.md
│       ├── student-task-manager-structured.md
│       ├── todo-list-iterative.md
│       ├── todo-list-simple.md
│       └── todo-list-structured.md
├── baseline
│   ├── student-task-manager-baseline.md
│   └── todo-list-baseline.md
├── comparison
│   ├── student-task-manager-requirements-comparison.md
│   └── todo-list-requirements-comparison.md
├── evaluation
│   ├── results_metrics_evaluation.xlsx
│   ├── evaluation-criteria.md
│   └── final-evaluation.md
├── presentation
│   ├── presentation-structure.md
│   ├── slides-notes.md
│   └── workflow.drawio
├── prompts
│   ├── iterative-prompt.md
│   ├── simple-prompt.md
│   └── structured-prompt.md
├── PROPOSAL.md
└── README.md
```

## Wichtige Dateien und Ordner

| Datei / Ordner | Inhalt |
|---|---|
| `PROPOSAL.md` | Projektidee, Ziel, Methodik und geplanter Workflow |
| `README.md` | Überblick über das gesamte Projekt |
| `prompts/` | Verwendete Prompt-Templates und Prompt-Strategien |
| `prompts/simple-prompt.md` | Beschreibung des einfachen Prompts |
| `prompts/structured-prompt.md` | Beschreibung des strukturierten Prompts |
| `prompts/iterative-prompt.md` | Beschreibung des iterativen Prompt-Vorgehens |
| `baseline/` | Manuell erstellte Baselines ohne KI-Unterstützung |
| `baseline/todo-list-baseline.md` | Manuelle Baseline für die Simple To-do List |
| `baseline/student-task-manager-baseline.md` | Manuelle Baseline für den Student Task Manager |
| `ai-results/chatgpt/` | Von ChatGPT generierte Requirements und User Stories |
| `ai-results/gemini/` | Von Gemini generierte Requirements und User Stories |
| `comparison/` | Vergleich zwischen manueller Baseline und KI-Ergebnissen |
| `comparison/todo-list-requirements-comparison.md` | Vergleich der Ergebnisse zur Simple To-do List |
| `comparison/student-task-manager-requirements-comparison.md` | Vergleich der Ergebnisse zum Student Task Manager |
| `evaluation/` | Bewertung, Kriterien und tabellarische Auswertung |
| `evaluation/evaluation-criteria.md` | Kriterien für die Bewertung der KI-Ergebnisse |
| `evaluation/final-evaluation.md` | Abschließende Bewertung des Projekts |
| `evaluation/results_metrics_evaluation.xlsx` | Tabellarische Auswertung der Ergebnisse und Metriken |
| `presentation/` | Materialien für die Präsentation |
| `presentation/presentation-structure.md` | Geplante Struktur der Präsentation |
| `presentation/slides-notes.md` | Notizen für die Präsentation |
| `presentation/workflow.drawio` | Visuelle Darstellung des Projekt-Workflows |

## Manuelle Baseline

Für beide Anwendungsideen wurde zuerst eine manuelle Baseline erstellt. Diese enthält die wichtigsten Requirements und User Stories, die ohne KI-Unterstützung formuliert wurden.

Die Baseline für die Simple To-do List enthält grundlegende Funktionen wie Aufgaben erstellen, bearbeiten, löschen, als erledigt markieren und offene sowie erledigte Aufgaben anzeigen.

Die Baseline für den Student Task Manager enthält zusätzlich Funktionen wie Kurszuordnung und Fälligkeitsdatum, bleibt aber ebenfalls relativ einfach.

## Vergleichskriterien

Die KI-Ergebnisse wurden anhand fester Kriterien bewertet:

- Abdeckung der manuellen Baseline
- zusätzliche sinnvolle Anforderungen
- fehlende Punkte
- Verständlichkeit
- Konkretheit
- Struktur
- Fehler oder unrealistische Annahmen
- Nutzen für Anfänger

Dabei wurde nicht nur geprüft, ob die KI dieselben Punkte wie die Baseline erkennt, sondern auch, ob sie sinnvolle neue Aspekte ergänzt.

## Metriken und Workflow-Darstellung

Zusätzlich zur Markdown-Dokumentation wurden zwei Dateien zur besseren Auswertung und Visualisierung ergänzt:

- Die Datei `evaluation/Auswertung_Ergebnisse_Metriken.xlsx` enthält eine tabellarische Auswertung der Ergebnisse und Metriken. Dort werden unter anderem die Anzahl der Turns, funktionale Requirements, nicht-funktionale Requirements, User Stories, Akzeptanzkriterien und zentrale Bewertungen festgehalten.
- Die Datei `presentation/workflow.drawio` zeigt den Projekt-Workflow visuell. Sie stellt die einzelnen Projektschritte von der Auswahl der Anwendungsideen bis zur Evaluation und Präsentation dar.

## Ergebnisse und Fazit

Die detaillierten Ergebnisse befinden sich in den Dateien im Ordner `comparison/` und in der finalen Auswertung unter `evaluation/final-evaluation.md`.

Zusammenfassend zeigte sich, dass ChatGPT und Gemini deutlich ausführlichere Requirements und User Stories erzeugten als die manuelle Baseline. Besonders strukturierte und iterative Prompts führten zu klareren und vollständigeren Ergebnissen.

ChatGPT lieferte besonders viele praktische Erweiterungen und ausführliche User Stories. Gemini wirkte teilweise formaler und stärker auf nicht-funktionale Requirements, Datenschutz, Barrierefreiheit und Akzeptanzkriterien fokussiert.

Gleichzeitig wurde deutlich, dass KI-Ergebnisse nicht ungeprüft übernommen werden sollten. Beide Systeme ergänzten teilweise Anforderungen, die für den eigentlichen Projektumfang zu groß oder zu technisch waren.

Das wichtigste Ergebnis des Projekts ist daher:

> KI ist hilfreich für Ideenfindung, Strukturierung und erste Requirements, ersetzt aber keine fachliche Prüfung durch Menschen.

## Lessons Learned

Aus dem Projekt ergeben sich folgende Erkenntnisse:

- Kurze Prompts liefern schnelle, aber oft unvollständige Ergebnisse.
- Strukturierte Prompts verbessern die Qualität deutlich.
- Iteratives Arbeiten mit KI führt zu den besten Ergebnissen.
- KI erkennt viele Aspekte, die in einer manuellen Baseline fehlen.
- KI neigt teilweise dazu, den Projektumfang zu stark zu erweitern.
- Menschliche Bewertung bleibt notwendig, um Requirements realistisch einzugrenzen.

## Präsentation

Für das Projekt ist eine ca. 20-minütige Präsentation vorgesehen. Die Präsentation behandelt die Projektidee, das Vorgehen, die verwendeten Prompts, die Ergebnisse der KI-Systeme, den Vergleich mit der Baseline und das abschließende Fazit.

Die zentrale Kernaussage der Präsentation lautet:

> KI kann bei der Erstellung von Requirements und User Stories sinnvoll unterstützen, ersetzt aber keine fachliche Prüfung.

## Autor:innen

- Patrick Boettger
- Lukas Berghofer

## Verwendete Technologien

- ChatGPT
- Gemini
- Markdown
- GitHub
- draw.io
- Excel