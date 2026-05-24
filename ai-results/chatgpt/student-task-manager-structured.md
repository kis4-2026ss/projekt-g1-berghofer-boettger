# ChatGPT Ergebnis: Student Task Manager - Structured Prompt

## Verwendeter Prompt

Erstelle Requirements und User Stories für eine einfache App, mit der Studierende Aufgaben für verschiedene Kurse verwalten können.

Berücksichtige dabei:

- funktionale Requirements
- nicht-funktionale Requirements
- User Stories im Format: Als Student möchte ich ..., damit ...
- eine klare und übersichtliche Struktur

## Ergebnis

# Requirements und User Stories  
## App zur Verwaltung von Aufgaben für Studierende

---

# 1. Projektübersicht

Die App soll Studierenden ermöglichen, Aufgaben und Abgaben für verschiedene Kurse einfach zu verwalten.  
Ziel ist es, den Überblick über Deadlines, Prioritäten und den Bearbeitungsstatus zu verbessern.

---

# 2. Funktionale Requirements

## 2.1 Benutzerverwaltung
- Die App soll es Studierenden ermöglichen, ein Benutzerkonto zu erstellen.
- Die App soll Login und Logout unterstützen.
- Die App soll persönliche Profildaten speichern können.

## 2.2 Kursverwaltung
- Studierende sollen Kurse anlegen können.
- Studierende sollen Kurse bearbeiten und löschen können.
- Jeder Kurs soll einen Namen und optional eine Beschreibung besitzen.

## 2.3 Aufgabenverwaltung
- Studierende sollen Aufgaben zu einem Kurs hinzufügen können.
- Aufgaben sollen folgende Informationen enthalten:
  - Titel
  - Beschreibung
  - Fälligkeitsdatum
  - Priorität
  - Bearbeitungsstatus
- Aufgaben sollen bearbeitet und gelöscht werden können.

## 2.4 Statusverwaltung
- Aufgaben sollen unterschiedliche Status besitzen:
  - Offen
  - In Bearbeitung
  - Erledigt
- Der Status soll jederzeit geändert werden können.

## 2.5 Erinnerungen und Benachrichtigungen
- Die App soll Erinnerungen für bevorstehende Deadlines senden können.
- Studierende sollen Erinnerungen aktivieren oder deaktivieren können.

## 2.6 Übersicht und Filter
- Die App soll alle Aufgaben übersichtlich anzeigen.
- Aufgaben sollen nach:
  - Kurs
  - Priorität
  - Fälligkeitsdatum
  - Status
  gefiltert werden können.

## 2.7 Kalenderansicht
- Die App soll eine Kalenderansicht für Deadlines bereitstellen.

---

# 3. Nicht-funktionale Requirements

## 3.1 Benutzerfreundlichkeit
- Die Benutzeroberfläche soll intuitiv und einfach bedienbar sein.
- Wichtige Funktionen sollen mit maximal drei Klicks erreichbar sein.

## 3.2 Performance
- Die App soll Aufgabenlisten innerhalb von 2 Sekunden laden.
- Änderungen sollen ohne spürbare Verzögerung gespeichert werden.

## 3.3 Sicherheit
- Benutzerdaten sollen sicher gespeichert werden.
- Passwörter sollen verschlüsselt gespeichert werden.
- Die App soll Datenschutzrichtlinien einhalten.

## 3.4 Verfügbarkeit
- Die App soll auf mobilen Geräten und Desktop-Geräten nutzbar sein.
- Die Anwendung soll eine hohe Verfügbarkeit gewährleisten.

## 3.5 Wartbarkeit
- Der Code soll modular aufgebaut sein.
- Neue Funktionen sollen einfach erweiterbar sein.

## 3.6 Zuverlässigkeit
- Daten sollen regelmäßig gespeichert werden.
- Datenverlust soll vermieden werden.

---

# 4. User Stories

## Benutzerkonto
- Als Student möchte ich ein Benutzerkonto erstellen können, damit meine Aufgaben gespeichert werden.
- Als Student möchte ich mich anmelden können, damit ich auf meine persönlichen Daten zugreifen kann.

## Kurse verwalten
- Als Student möchte ich Kurse anlegen können, damit ich meine Aufgaben organisieren kann.
- Als Student möchte ich Kurse bearbeiten oder löschen können, damit meine Kursliste aktuell bleibt.

## Aufgaben verwalten
- Als Student möchte ich Aufgaben hinzufügen können, damit ich keine Abgaben vergesse.
- Als Student möchte ich Aufgaben bearbeiten können, damit Informationen aktuell bleiben.
- Als Student möchte ich Aufgaben löschen können, damit erledigte oder unnötige Aufgaben entfernt werden.

## Aufgabenstatus
- Als Student möchte ich den Status einer Aufgabe ändern können, damit ich meinen Fortschritt verfolgen kann.

## Erinnerungen
- Als Student möchte ich Erinnerungen erhalten, damit ich wichtige Deadlines nicht verpasse.
- Als Student möchte ich Erinnerungen deaktivieren können, damit ich selbst entscheiden kann, wann ich benachrichtigt werde.

## Übersicht und Filter
- Als Student möchte ich Aufgaben nach Kurs filtern können, damit ich mich auf ein bestimmtes Fach konzentrieren kann.
- Als Student möchte ich Aufgaben nach Priorität sortieren können, damit ich wichtige Aufgaben zuerst sehe.
- Als Student möchte ich eine Kalenderansicht nutzen können, damit ich Deadlines zeitlich planen kann.

---

# 5. Mögliche Erweiterungen

- Synchronisation mit Hochschulplattformen
- Gemeinsame Gruppenaufgaben
- Dark Mode
- Push-Benachrichtigungen
- Export von Aufgaben in Kalender-Apps
- KI-basierte Priorisierung von Aufgaben