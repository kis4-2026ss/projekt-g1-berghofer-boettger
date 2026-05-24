# ChatGPT Ergebnis: Simple To-do List - Iterative Prompt

## Verwendete Prompts

### Prompt 1

Erstelle Requirements und User Stories für eine einfache To-do-Listen-App.

### Prompt 2

Überarbeite das Ergebnis und ergänze fehlende funktionale und nicht-funktionale Requirements.

### Prompt 3

Verbessere die User Stories und achte darauf, dass sie im Format „Als Benutzer möchte ich ..., damit ...“ geschrieben sind.

## Ergebnis

# 4. User Stories

## Epic: Aufgabenverwaltung

---

## US-01 Aufgabe erstellen

**Als Benutzer möchte ich neue Aufgaben erstellen können, damit ich meine Aufgaben und Aktivitäten festhalten kann.**

### Akzeptanzkriterien
- Ein Eingabefeld für den Titel ist vorhanden.
- Der Titel ist ein Pflichtfeld.
- Optional können Beschreibung, Priorität und Fälligkeitsdatum angegeben werden.
- Nach dem Speichern erscheint die Aufgabe sofort in der Aufgabenliste.
- Die Aufgabe wird dauerhaft gespeichert.

---

## US-02 Aufgaben anzeigen

**Als Benutzer möchte ich alle meine Aufgaben in einer übersichtlichen Liste sehen, damit ich den Überblick über offene und erledigte Aufgaben behalten kann.**

### Akzeptanzkriterien
- Alle gespeicherten Aufgaben werden angezeigt.
- Erledigte Aufgaben sind visuell gekennzeichnet.
- Die Liste zeigt mindestens Titel und Status an.

---

## US-03 Aufgabe bearbeiten

**Als Benutzer möchte ich bestehende Aufgaben bearbeiten können, damit ich Informationen aktualisieren oder korrigieren kann.**

### Akzeptanzkriterien
- Titel und Beschreibung können geändert werden.
- Priorität und Fälligkeitsdatum können angepasst werden.
- Änderungen werden automatisch gespeichert.
- Die aktualisierten Informationen werden sofort angezeigt.

---

## US-04 Aufgabe als erledigt markieren

**Als Benutzer möchte ich Aufgaben als erledigt markieren können, damit ich abgeschlossene Aufgaben von offenen unterscheiden kann.**

### Akzeptanzkriterien
- Aufgaben besitzen eine Checkbox oder einen Toggle.
- Der Status wird sofort aktualisiert.
- Erledigte Aufgaben werden visuell hervorgehoben.

---

## US-05 Aufgabe wieder öffnen

**Als Benutzer möchte ich erledigte Aufgaben wieder als offen markieren können, damit ich versehentlich abgeschlossene Aufgaben erneut bearbeiten kann.**

### Akzeptanzkriterien
- Bereits erledigte Aufgaben können reaktiviert werden.
- Der Status wechselt wieder auf „offen“.
- Die visuelle Kennzeichnung wird entfernt.

---

## US-06 Aufgabe löschen

**Als Benutzer möchte ich Aufgaben löschen können, damit ich nicht mehr benötigte Aufgaben entfernen kann.**

### Akzeptanzkriterien
- Jede Aufgabe besitzt eine Löschfunktion.
- Vor dem Löschen erscheint eine Bestätigung.
- Nach dem Löschen verschwindet die Aufgabe sofort aus der Liste.

---

## US-07 Aufgaben filtern

**Als Benutzer möchte ich Aufgaben nach ihrem Status filtern können, damit ich mich auf relevante Aufgaben konzentrieren kann.**

### Akzeptanzkriterien
- Es gibt Filter für:
  - Alle
  - Offen
  - Erledigt
- Die Liste aktualisiert sich sofort nach Auswahl eines Filters.

---

## US-08 Aufgaben durchsuchen

**Als Benutzer möchte ich Aufgaben durchsuchen können, damit ich bestimmte Aufgaben schneller finde.**

### Akzeptanzkriterien
- Die Suche funktioniert über Titel und Beschreibung.
- Suchergebnisse aktualisieren sich dynamisch während der Eingabe.

---

## US-09 Aufgaben sortieren

**Als Benutzer möchte ich Aufgaben sortieren können, damit ich meine Aufgaben besser organisieren kann.**

### Akzeptanzkriterien
- Aufgaben können sortiert werden nach:
  - Erstellungsdatum
  - Fälligkeitsdatum
  - Priorität
  - Alphabetisch
- Die Anzeige wird sofort aktualisiert.

---

## US-10 Prioritäten vergeben

**Als Benutzer möchte ich Prioritäten für Aufgaben festlegen können, damit ich wichtige Aufgaben schneller erkenne.**

### Akzeptanzkriterien
- Prioritäten auswählbar:
  - Niedrig
  - Mittel
  - Hoch
- Die Priorität wird sichtbar dargestellt.

---

## US-11 Fälligkeitsdatum festlegen

**Als Benutzer möchte ich ein Fälligkeitsdatum für Aufgaben festlegen können, damit ich Fristen besser einhalten kann.**

### Akzeptanzkriterien
- Ein Datum kann ausgewählt werden.
- Das Fälligkeitsdatum wird in der Aufgabenliste angezeigt.

---

## US-12 Mehrere Aufgaben gleichzeitig verwalten

**Als Benutzer möchte ich mehrere Aufgaben gleichzeitig auswählen können, damit ich wiederkehrende Aktionen schneller durchführen kann.**

### Akzeptanzkriterien
- Mehrere Aufgaben können markiert werden.
- Sammelaktionen sind möglich:
  - Löschen
  - Als erledigt markieren

---

## US-13 Aufgaben dauerhaft speichern

**Als Benutzer möchte ich, dass meine Aufgaben nach dem Schließen der Anwendung erhalten bleiben, damit ich meine Daten nicht verliere.**

### Akzeptanzkriterien
- Aufgaben werden lokal gespeichert.
- Nach dem erneuten Öffnen der Anwendung werden die Aufgaben automatisch geladen.

---

## US-14 Anwendung mobil nutzen

**Als Benutzer möchte ich die Anwendung auf mobilen Geräten nutzen können, damit ich meine Aufgaben auch unterwegs verwalten kann.**

### Akzeptanzkriterien
- Die Benutzeroberfläche passt sich mobilen Geräten an.
- Inhalte sind ohne horizontales Scrollen nutzbar.
- Buttons und Eingabefelder sind touchfreundlich.

---

## US-15 Anwendung per Tastatur bedienen

**Als Benutzer möchte ich die Anwendung mit der Tastatur bedienen können, damit ich schneller und barrierefrei arbeiten kann.**

### Akzeptanzkriterien
- Aufgaben können per Enter-Taste gespeichert werden.
- Navigation per Tab-Taste funktioniert korrekt.
- Interaktive Elemente besitzen sichtbare Fokuszustände.

---

## US-16 Leere Zustände verstehen

**Als Benutzer möchte ich informative Hinweise sehen, wenn keine Aufgaben vorhanden sind, damit ich den aktuellen Zustand der Anwendung besser verstehe.**

### Akzeptanzkriterien
- Bei leerer Aufgabenliste erscheint ein Hinweis.
- Unterschiedliche Hinweise werden für:
  - keine Aufgaben
  - keine offenen Aufgaben
  - keine erledigten Aufgaben
  angezeigt.

---

## US-17 Fehler verständlich angezeigt bekommen

**Als Benutzer möchte ich verständliche Fehlermeldungen erhalten, damit ich Eingabefehler schnell korrigieren kann.**

### Akzeptanzkriterien
- Fehlende Pflichtfelder werden erklärt.
- Fehlermeldungen sind klar und verständlich formuliert.
- Fehler werden visuell hervorgehoben.