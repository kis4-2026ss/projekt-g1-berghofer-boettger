# Vergleich: Student Task Manager

In diesem Vergleich werden die manuelle Baseline und die KI-generierten Ergebnisse gegenübergestellt.

## Vergleichskriterien

| Kriterium | Manuelle Baseline | ChatGPT | Gemini |
|---|---|---|---|
| Funktionale Requirements | Enthält die Grundfunktionen: Aufgaben erstellen, Kurs zuordnen, Fälligkeitsdatum festlegen, bearbeiten, löschen, erledigen und anzeigen. | Deutlich ausführlicher. Enthält zusätzlich Benutzerkonto, Login, Kursverwaltung, Prioritäten, Statusverwaltung, Erinnerungen, Kalenderansicht, Filter, Sortierung und teilweise Dashboard-Funktionen. | Ebenfalls deutlich ausführlicher. Enthält zusätzlich Kursfarben, Prioritäten, Benachrichtigungen, Dashboard, Offline-Funktionalität, Kalenderansicht, Synchronisation und genauere Datenfelder. |
| Nicht-funktionale Requirements | Nicht separat ausgearbeitet. | Enthält Benutzerfreundlichkeit, Performance, Sicherheit, responsives Design, Verfügbarkeit, Wartbarkeit und Zuverlässigkeit. | Enthält Usability, Performance, Offline-Nutzung, Responsiveness, Sicherheit, Datenschutz, Barrierefreiheit und Synchronisation. |
| User Stories | Enthält einfache User Stories für die wichtigsten Grundfunktionen. | Enthält viele User Stories, besonders im iterativen Prompt. Diese decken Benutzerkonto, Kurse, Aufgaben, Status, Dashboard, Erinnerungen, Kalender und Datenmanagement ab. | Enthält strukturierte User Stories mit Akzeptanzkriterien. Besonders stark sind Kursorganisation, Aufgabenverwaltung, Dashboard, Benachrichtigungen, Kalender und Datenschutz ausgearbeitet. |
| Fehlende Punkte | Es fehlen nicht-funktionale Requirements, Akzeptanzkriterien, Erinnerungen, Prioritäten, Filter, Kalender und Sicherheitsaspekte. | Im Simple und Structured Prompt brauchbar. Der iterative Prompt enthält aber fast nur User Stories und keine vollständige erneute Requirements-Struktur. | Sehr vollständig, aber teilweise deutlich über eine einfache App hinausgehend. Einige Anforderungen sind für ein kleines Projekt zu detailliert. |
| Zusätzliche sinnvolle Punkte | Keine größeren Ergänzungen über die Grundidee hinaus. | Sinnvolle Ergänzungen: Login, Kursverwaltung, Prioritäten, Erinnerungen, Filter, Kalender, Dashboard, Passwort zurücksetzen, Datenexport und Datensicherung. | Sinnvolle Ergänzungen: Kursfarben, Offline-Modus, Push-Benachrichtigungen, Kalenderansicht, Synchronisation, Datenschutz, Barrierefreiheit und Akzeptanzkriterien. |
| Auffällige Fehler | Keine fachlichen Fehler, aber sehr knapp. | Der iterative Prompt wird sehr umfangreich und entfernt sich teilweise vom einfachen Projektumfang. Einige Features wie Datei-Uploads, Gruppenprojekte oder KI-Priorisierung wirken eher wie Erweiterungen. | Teilweise zu konkrete technische Vorgaben, z. B. OAuth, TLS-Version, WCAG, Offline-First und Cloud-Synchronisation. Das ist fachlich sinnvoll, aber für eine einfache App eventuell zu groß. |

## Kurze Bewertung

Die KI-generierten Ergebnisse sind deutlich vollständiger als die manuelle Baseline. Beide KI-Systeme erkennen sinnvolle Zusatzfunktionen wie Prioritäten, Erinnerungen, Filter und Kalenderansichten.

ChatGPT liefert besonders im iterativen Prompt sehr viele User Stories und deckt viele mögliche Funktionen ab. Dadurch entsteht ein breiter Funktionsumfang, der aber teilweise über eine einfache Anwendung hinausgeht.

Gemini wirkt stärker wie ein formales Requirements-Dokument. Die Ergebnisse enthalten oft genauere Akzeptanzkriterien, Prioritäten und nicht-funktionale Anforderungen. Gleichzeitig werden teilweise sehr konkrete technische Vorgaben ergänzt, die nicht direkt aus der ursprünglichen Aufgabenstellung hervorgehen.

Für den Student Task Manager sind beide KI-Ergebnisse brauchbar. Gemini wirkt strukturierter, ChatGPT liefert dafür mehr Breite bei den User Stories. Beide Ergebnisse müssen fachlich geprüft und auf den gewünschten Projektumfang reduziert werden.