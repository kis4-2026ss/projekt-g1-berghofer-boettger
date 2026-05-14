## Project Proposal: AI-assisted Requirements & User Stories Generator

## 1. Goal of the Project

Das Ziel des Projekts ist zu untersuchen, wie gut KI eine Person ohne Programmier- oder Software-Engineering-Erfahrung dabei unterstützen kann, aus einer einfachen Softwareidee brauchbare Requirements und User Stories zu erstellen.

Viele unerfahrene Personen haben zwar eine Idee für ein Programm, wissen aber nicht, welche Anforderungen, Sonderfälle, Nutzerrollen, technischen Einschränkungen oder Qualitätsaspekte für eine vollständige Umsetzung relevant sind. Genau hier soll KI unterstützen.

Im Projekt wird daher getestet, ob ein KI-gestützter Workflow aus einer groben Beschreibung systematisch Requirements und User Stories ableiten kann, die auch für eine unerfahrene Person verständlich und hilfreich sind.

## 2. System / Workflow to be Developed

Es wird kein komplexes Softwareprodukt entwickelt, sondern ein dokumentierter KI-gestützter Workflow.

Der Workflow besteht aus folgenden Schritten:

1. Auswahl mehrerer Anwendungsideen mit unterschiedlicher Komplexität.
2. Erstellung einer manuellen Baseline ohne KI-Unterstützung.
3. Generierung von Requirements und User Stories mit ChatGPT und Gemini.
4. Vergleich der KI-Ergebnisse mit der manuellen Baseline.
5. Strukturierte Selbstevaluierung aus Sicht einer Person mit wenig bis keiner ursprünglichen Software-Engineering-Erfahrung.
6. Dokumentation der Ergebnisse, Prompts, Chatverläufe und Metriken.

Als Anwendungsideen werden voraussichtlich verwendet:

| Anwendungsidee | Komplexität | Beschreibung |
|---|---|---|
| Simple To-do List | Niedrig | Eine einfache App zum Erstellen, Bearbeiten und Abhaken von Aufgaben |
| Student Task Manager | Mittel | Eine App zur Verwaltung von Aufgaben, Deadlines, Kursen und Lernfortschritt |

Durch zwei Anwendungsideen soll geprüft werden, ob die Qualität der KI-Ergebnisse von der Komplexität der Ausgangsidee abhängt.

## 3. AI Assistance

ChatGPT und Gemini werden genutzt, um:

- aus einer unklaren Idee strukturierte Requirements zu erstellen,
- fehlende Aspekte und Edge Cases vorzuschlagen,
- User Stories mit Akzeptanzkriterien zu formulieren,
- die Requirements auf Verständlichkeit und Vollständigkeit zu prüfen,
- eine einfache Priorisierung der Anforderungen vorzuschlagen.

Die KI-generierten Ergebnisse werden manuell geprüft und mit einer Baseline verglichen.

Zusätzlich werden verschiedene Prompt-Strategien getestet:

| Prompt-Strategie | Zweck |
|---|---|
| Einfacher Prompt | Prüfen, was ChatGPT aus einer sehr groben Beschreibung erzeugt |
| Strukturierter Prompt | Vorgabe eines festen Templates für Requirements und User Stories |
| Iterativer Prompt | KI stellt Rückfragen und verbessert die Ergebnisse schrittweise |

## 4. Baseline and Comparison Method

Um einen sinnvollen Vergleich durchführen zu können, wird vor der KI-Nutzung eine manuelle Baseline erstellt. Diese enthält Requirements und User Stories, die ohne KI-Unterstützung formuliert werden.

Danach werden die KI-generierten Ergebnisse mit dieser Baseline verglichen. Dabei wird nicht nur geprüft, ob die KI dieselben Punkte erkennt, sondern auch, ob sie sinnvolle zusätzliche Anforderungen ergänzt oder unrealistische Annahmen trifft.

| Kriterium | Fragestellung |
|---|---|
| Abdeckung | Welche Punkte aus der Baseline wurden von der KI erkannt? |
| Zusätzlicher Mehrwert | Welche sinnvollen Anforderungen ergänzt die KI? |
| Fehlende Punkte | Welche wichtigen Anforderungen fehlen in der KI-Version? |
| Verständlichkeit | Sind die Requirements und User Stories für Anfänger verständlich? |
| Konkretheit | Sind die Anforderungen konkret genug für eine spätere Umsetzung? |
| Struktur | Sind Requirements, User Stories und Akzeptanzkriterien logisch aufgebaut? |
| Fehler / Halluzinationen | Enthält die KI unrealistische oder falsche Annahmen? |

Die Ergebnisse werden in Tabellen dokumentiert und anschließend qualitativ zusammengefasst.

## 5. Evaluation Method

Eine externe Benutzerevaluierung mit 5–7 Personen ist im Rahmen dieses Projekts nicht vorgesehen, da die passende Zielgruppe schwer sinnvoll zu rekrutieren wäre. Die Personen müssten einerseits keine Software-Engineering-Erfahrung haben, andererseits aber genug Interesse und Zeit mitbringen, um Requirements und User Stories bewerten zu können.

Stattdessen wird eine strukturierte Selbstevaluierung durchgeführt. Dabei wird bewusst reflektiert, welche Aspekte einer Softwareidee aus heutiger Sicht durch das Studium bekannt sind und welche Punkte vor der Ausbildung vermutlich nicht bedacht worden wären.

Die Evaluation besteht aus drei Teilen:

| Schritt | Beschreibung |
|---|---|
| Manuelle Baseline | Requirements und User Stories werden zuerst ohne KI-Unterstützung erstellt |
| KI-generierte Version | ChatGPT und Gemini erstellt Requirements, User Stories und Akzeptanzkriterien auf Basis definierter Prompts |
| Vergleich und Reflexion | Beide Ergebnisse werden anhand fixer Kriterien verglichen und dokumentiert |

Zusätzlich wird bewertet, ob die KI einem Anfänger helfen würde, über wichtige Softwareaspekte nachzudenken, die über reine Basisfunktionen hinausgehen.

## 6. Reproducibility

Zur Sicherstellung der Reproduzierbarkeit werden alle relevanten Schritte dokumentiert.

| Aspekt | Dokumentation |
|---|---|
| Anwendungsideen | Ausgangsbeschreibungen der getesteten App-Ideen |
| Prompt-Templates | Verwendete System- und User-Prompts |
| Chatverläufe | Relevante KI-Ausgaben werden gespeichert |
| KI-Modell | Verwendetes Tool und Modell, soweit sichtbar |
| Prompt-Strategie | Einfacher, strukturierter oder iterativer Prompt |
| Metriken | Anzahl der Turns, Bearbeitungszeit, Anzahl der Requirements und User Stories |
| Vergleich | Manuelle Baseline, KI-Ergebnis und Bewertungstabelle |
| Reflexion | Dokumentation der wichtigsten Unterschiede und Erkenntnisse |

Dadurch soll nachvollziehbar sein, wie die Ergebnisse entstanden sind und wie der Vergleich durchgeführt wurde.

## 7. Validation

Die zentrale Validierungsfrage lautet:

**Wie hilfreich sind KI-generierte Requirements und User Stories für jemanden ohne Code-Erfahrung?**

Bewertet wird anhand folgender Kriterien:

| Kriterium | Fragestellung |
|---|---|
| Verständlichkeit | Kann eine unerfahrene Person die Requirements verstehen? |
| Vollständigkeit | Denkt die KI an wichtige Funktionen, Rollen und Sonderfälle? |
| Umsetzbarkeit | Sind die Anforderungen konkret genug für eine spätere Implementierung? |
| Struktur | Sind Requirements und User Stories logisch aufgebaut? |
| Mehrwert | Erkennt die KI Aspekte, an die ein Anfänger vermutlich nicht gedacht hätte? |
| Grenzen | Welche wichtigen Punkte fehlen oder sind zu ungenau? |

## 8. Project Plan

| Phase | Aufgabe |
|---|---|
| 1 | Anwendungsideen mit unterschiedlicher Komplexität auswählen |
| 2 | Manuelle Baseline für Requirements und User Stories erstellen |
| 3 | Prompt-Templates und Prompt-Strategien definieren |
| 4 | Requirements und User Stories mit ChatGPT generieren |
| 5 | KI-Ergebnisse mit der Baseline vergleichen |
| 6 | Metriken und Chatverläufe dokumentieren |
| 7 | Strukturierte Selbstevaluierung durchführen |
| 8 | Ergebnisse auswerten und README schreiben |
| 9 | Präsentation vorbereiten |

## 7. Teamwork and Responsibilities

| Teammitglied | Verantwortlichkeiten |
|---|---|
| Patrick Boettger | Definition der Ausgangsidee, Prompt-Workflow, KI-generierte Requirements, Prüfung auf Vollständigkeit und Verständlichkeit |
| Lukas Berghofer | KI-generierte User Stories, Akzeptanzkriterien, Evaluation der Ergebnisse, GitHub-Dokumentation |

## 9. Teamwork and Responsibilities

| Teammitglied | Verantwortlichkeiten |
|---|---|
| Patrick Boettger | Auswahl der Anwendungsideen, Erstellung der Baseline, Prompt-Workflow, Vergleich der Requirements |
| Lukas Berghofer | Generierung und Vergleich der User Stories, Akzeptanzkriterien, Evaluation, GitHub-Dokumentation |

## 10. Relation to Course

Das Projekt passt zum Kurs, weil es AI-assisted Software Engineering in der frühen Phase des Software Development Lifecycle untersucht. Der Fokus liegt auf Requirements Engineering, User Stories, Prompt Engineering, Evaluation von KI-Ergebnissen und Human-in-the-loop-Prüfung.

Im Kurs wird AI-assisted Software Engineering als Unterstützung über den gesamten Softwareentwicklungsprozess hinweg betrachtet. Besonders die frühe Planung, das Erstellen von Software Design Documents, das Ableiten von Requirements und das Generieren von User Stories sind passende Einsatzbereiche für LLMs.

## 11. Used Technologies

| Technology | Purpose |
|---|---|
| ChatGPT & Gemini | Generierung von Requirements und User Stories |
| GitHub | Repository und Projektdokumentation |
| Markdown | Proposal, README, Requirements, User Stories und Evaluation |
| draw.io | Darstellung des Workflows |
| Excel | Tabellarische Auswertung der Ergebnisse und Metriken |
