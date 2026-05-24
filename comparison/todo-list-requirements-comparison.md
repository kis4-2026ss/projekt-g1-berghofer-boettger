# Vergleich: Simple To-do List

In diesem Vergleich werden die manuelle Baseline und die KI-generierten Ergebnisse gegenübergestellt.

## Vergleichskriterien

| Kriterium | Manuelle Baseline | ChatGPT | Gemini |
|---|---|---|---|
| Funktionale Requirements | Enthält die wichtigsten Grundfunktionen: Aufgaben erstellen, bearbeiten, löschen, erledigen und anzeigen. | Deutlich ausführlicher. Enthält zusätzlich Filter, Sortierung, Fälligkeitsdatum, lokale Speicherung, Prioritäten und teilweise Massenaktionen. | Ebenfalls ausführlicher als die Baseline. Enthält zusätzlich lokale Speicherung, Wiederöffnen erledigter Aufgaben, Filterung, Sortierung und teilweise detaillierte Validierung. |
| Nicht-funktionale Requirements | Nicht explizit getrennt ausgearbeitet. | Enthält Benutzerfreundlichkeit, Performance, responsives Design, Datenschutz, Wartbarkeit und Erweiterbarkeit. | Enthält Benutzerfreundlichkeit, Performance, Barrierefreiheit, Datenschutz, Responsiveness und Cross-Browser-Kompatibilität. |
| User Stories | Enthält einfache User Stories für die wichtigsten Grundfunktionen. | Enthält mehr und detailliertere User Stories, besonders im iterativen Prompt. Die Akzeptanzkriterien sind teilweise sehr ausführlich. | Enthält ebenfalls detaillierte User Stories mit Akzeptanzkriterien. Besonders der iterative Prompt ergänzt viele konkrete Qualitätsanforderungen. |
| Fehlende Punkte | Es fehlen nicht-funktionale Requirements, Akzeptanzkriterien und genauere technische Rahmenbedingungen. | Im Simple Prompt noch etwas allgemein, später deutlich vollständiger. Teilweise werden Features ergänzt, die nicht direkt gefordert wurden. | Im Simple Prompt bereits recht strukturiert. Teilweise fehlen im Vergleich zu ChatGPT einzelne organisatorische Features wie Prioritäten, dafür sind Barrierefreiheit und Validierung stärker ausgearbeitet. |
| Zusätzliche sinnvolle Punkte | Keine größeren Ergänzungen über die Grundidee hinaus. | Sinnvolle Ergänzungen: Local Storage, responsives Design, Fälligkeitsdatum, Sortierung, Prioritäten, Suche, Tastaturbedienung und Fehlerhinweise. | Sinnvolle Ergänzungen: Local Storage, Validierung leerer Eingaben, Undo beim Löschen, Barrierefreiheit, Screenreader-Unterstützung und XSS-Schutz. |
| Auffällige Fehler | Keine fachlichen Fehler, aber sehr knapp. | Teilweise zu umfangreich für eine einfache To-do-Listen-App. Der iterative Prompt enthält viele Erweiterungen, die eher über ein MVP hinausgehen. | Teilweise sehr konkrete technische Vorgaben, z. B. genaue Ladezeiten oder WCAG-Vorgaben. Diese sind sinnvoll, aber für eine einfache App eventuell zu detailliert. |

## Kurze Bewertung

Die KI-generierten Ergebnisse sind deutlich vollständiger als die manuelle Baseline. Besonders strukturierte und iterative Prompts führen zu besseren Ergebnissen, weil sie funktionale und nicht-funktionale Requirements klarer trennen und zusätzlich Akzeptanzkriterien liefern.

ChatGPT liefert viele praktische Erweiterungen und sehr ausführliche User Stories. Gemini wirkt teilweise stärker auf Qualität, Barrierefreiheit, Datenschutz und technische Rahmenbedingungen fokussiert.

Für eine einfache To-do-Listen-App sind beide KI-Ergebnisse brauchbar. Die Ergebnisse müssen aber fachlich geprüft werden, weil beide Systeme teilweise zusätzliche Funktionen vorschlagen, die über die ursprüngliche einfache Anwendungsidee hinausgehen.