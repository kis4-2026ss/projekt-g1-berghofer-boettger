# ChatGPT Ergebnis: Simple To-do List - Structured Prompt

## Verwendeter Prompt

Erstelle Requirements und User Stories für eine einfache To-do-Listen-App.

Berücksichtige dabei:

- funktionale Requirements
- nicht-funktionale Requirements
- User Stories im Format: Als Benutzer möchte ich ..., damit ...
- eine klare und übersichtliche Struktur

## Ergebnis

# Requirements und User Stories – To-do-Listen-App

## 1. Projektübersicht

Die To-do-Listen-App soll Benutzern ermöglichen, Aufgaben einfach zu erstellen, zu verwalten und nachzuverfolgen.  
Der Fokus liegt auf einer intuitiven Bedienung und einer übersichtlichen Darstellung der Aufgaben.

---

# 2. Funktionale Requirements

## 2.1 Aufgabenverwaltung

### FR-01: Aufgabe erstellen
Der Benutzer kann neue Aufgaben anlegen.

### FR-02: Aufgabe bearbeiten
Der Benutzer kann bestehende Aufgaben bearbeiten.

### FR-03: Aufgabe löschen
Der Benutzer kann Aufgaben entfernen.

### FR-04: Aufgabe als erledigt markieren
Der Benutzer kann Aufgaben als erledigt kennzeichnen.

### FR-05: Aufgabenliste anzeigen
Die Anwendung zeigt alle vorhandenen Aufgaben in einer Liste an.

### FR-06: Aufgabenstatus anzeigen
Die Anwendung zeigt an, ob eine Aufgabe offen oder erledigt ist.

### FR-07: Aufgaben filtern
Der Benutzer kann Aufgaben nach Status filtern:
- Alle
- Offen
- Erledigt

### FR-08: Aufgaben sortieren
Die Anwendung ermöglicht die Sortierung nach:
- Erstellungsdatum
- Fälligkeitsdatum
- Status

### FR-09: Fälligkeitsdatum festlegen
Der Benutzer kann einer Aufgabe ein Fälligkeitsdatum zuweisen.

### FR-10: Datenspeicherung
Die Aufgaben werden persistent gespeichert, sodass sie nach dem Neustart der Anwendung erhalten bleiben.

---

# 3. Nicht-funktionale Requirements

## 3.1 Benutzerfreundlichkeit

### NFR-01: Einfache Bedienung
Die Benutzeroberfläche soll intuitiv und leicht verständlich sein.

### NFR-02: Responsives Design
Die Anwendung soll auf Desktop-, Tablet- und Mobilgeräten nutzbar sein.

---

## 3.2 Performance

### NFR-03: Schnelle Ladezeiten
Die Anwendung soll innerhalb von maximal 2 Sekunden geladen werden.

### NFR-04: Reaktionszeit
Benutzeraktionen sollen innerhalb von 1 Sekunde verarbeitet werden.

---

## 3.3 Sicherheit

### NFR-05: Datenschutz
Benutzerdaten dürfen nicht unautorisiert zugänglich sein.

### NFR-06: Sichere Speicherung
Gespeicherte Daten sollen vor Verlust geschützt werden.

---

## 3.4 Wartbarkeit

### NFR-07: Erweiterbarkeit
Die Softwarearchitektur soll zukünftige Erweiterungen ermöglichen.

### NFR-08: Codequalität
Der Quellcode soll dokumentiert und modular aufgebaut sein.

---

# 4. User Stories

## Aufgaben erstellen und verwalten

### US-01
Als Benutzer möchte ich neue Aufgaben erstellen können, damit ich meine Tätigkeiten festhalten kann.

### US-02
Als Benutzer möchte ich Aufgaben bearbeiten können, damit ich Änderungen an meinen Aufgaben vornehmen kann.

### US-03
Als Benutzer möchte ich Aufgaben löschen können, damit ich nicht mehr benötigte Aufgaben entfernen kann.

### US-04
Als Benutzer möchte ich Aufgaben als erledigt markieren können, damit ich meinen Fortschritt verfolgen kann.

---

## Übersicht und Organisation

### US-05
Als Benutzer möchte ich alle Aufgaben in einer übersichtlichen Liste sehen, damit ich meine Aufgaben schnell erfassen kann.

### US-06
Als Benutzer möchte ich Aufgaben filtern können, damit ich nur relevante Aufgaben angezeigt bekomme.

### US-07
Als Benutzer möchte ich Aufgaben sortieren können, damit ich meine Aufgaben besser organisieren kann.

### US-08
Als Benutzer möchte ich Fälligkeitsdaten für Aufgaben festlegen können, damit ich wichtige Termine nicht vergesse.

---

## Nutzung und Bedienung

### US-09
Als Benutzer möchte ich die Anwendung auf verschiedenen Geräten nutzen können, damit ich jederzeit Zugriff auf meine Aufgaben habe.

### US-10
Als Benutzer möchte ich eine schnell reagierende Anwendung verwenden, damit ich effizient arbeiten kann.

---

# 5. Akzeptanzkriterien (Beispiele)

## AK-01: Aufgabe erstellen
- Eine neue Aufgabe kann über ein Eingabefeld hinzugefügt werden.
- Nach dem Speichern erscheint die Aufgabe sofort in der Liste.

## AK-02: Aufgabe abschließen
- Erledigte Aufgaben werden visuell markiert.
- Der Status bleibt nach dem Neuladen erhalten.

## AK-03: Aufgaben filtern
- Der Benutzer kann zwischen „Alle“, „Offen“ und „Erledigt“ wechseln.
- Die Liste aktualisiert sich entsprechend der Auswahl.

---

# 6. Mögliche Erweiterungen

- Benutzerkonten und Login
- Synchronisation über Cloud-Dienste
- Erinnerungen und Benachrichtigungen
- Kategorien und Tags
- Dark Mode
- Drag-and-drop-Sortierung