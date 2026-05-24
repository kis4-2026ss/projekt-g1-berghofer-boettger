# ChatGPT Ergebnis: Student Task Manager - Simple Prompt

## Verwendeter Prompt

Erstelle Requirements und User Stories für eine einfache App, mit der Studierende Aufgaben für verschiedene Kurse verwalten können.

## Ergebnis

# Studienaufgaben-App – Requirements & User Stories

## 1. Projektübersicht

Die App soll Studierenden ermöglichen, Aufgaben und Abgaben für verschiedene Kurse einfach zu verwalten.  
Ziel ist eine übersichtliche und intuitive Anwendung zur Organisation des Studienalltags.

---

# 2. Funktionale Anforderungen

## 2.1 Benutzerverwaltung

### FR-01 Registrierung
Die App soll es neuen Benutzer:innen ermöglichen, ein Konto zu erstellen.

### FR-02 Login
Benutzer:innen sollen sich mit E-Mail und Passwort anmelden können.

### FR-03 Logout
Benutzer:innen sollen sich sicher abmelden können.

---

## 2.2 Kursverwaltung

### FR-04 Kurse erstellen
Benutzer:innen sollen neue Kurse anlegen können.

### FR-05 Kurse bearbeiten
Benutzer:innen sollen Kursnamen und Informationen ändern können.

### FR-06 Kurse löschen
Benutzer:innen sollen Kurse entfernen können.

### FR-07 Kursübersicht
Die App soll alle Kurse in einer übersichtlichen Liste anzeigen.

---

## 2.3 Aufgabenverwaltung

### FR-08 Aufgaben erstellen
Benutzer:innen sollen Aufgaben einem Kurs zuordnen und erstellen können.

### FR-09 Aufgaben bearbeiten
Benutzer:innen sollen Titel, Beschreibung, Fälligkeitsdatum und Status ändern können.

### FR-10 Aufgaben löschen
Benutzer:innen sollen Aufgaben entfernen können.

### FR-11 Aufgabenstatus
Aufgaben sollen als:
- Offen
- In Bearbeitung
- Erledigt

markiert werden können.

### FR-12 Aufgabenübersicht
Die App soll Aufgaben nach:
- Kurs
- Fälligkeitsdatum
- Status

filtern und sortieren können.

---

## 2.4 Benachrichtigungen

### FR-13 Erinnerungen
Die App soll Benutzer:innen an bevorstehende Abgaben erinnern.

### FR-14 Deadline-Warnung
Die App soll Aufgaben hervorheben, deren Deadline bald erreicht ist.

---

# 3. Nicht-funktionale Anforderungen

## NFR-01 Benutzerfreundlichkeit
Die Oberfläche soll einfach und intuitiv bedienbar sein.

## NFR-02 Performance
Seiten und Listen sollen innerhalb von maximal 2 Sekunden geladen werden.

## NFR-03 Sicherheit
Passwörter sollen verschlüsselt gespeichert werden.

## NFR-04 Responsives Design
Die App soll auf Smartphone, Tablet und Desktop funktionieren.

## NFR-05 Verfügbarkeit
Die App soll rund um die Uhr verfügbar sein.

---

# 4. User Stories

## Epic: Benutzerverwaltung

### US-01 Registrierung
Als Studierende:r  
möchte ich ein Konto erstellen können,  
damit meine Aufgaben gespeichert werden.

### US-02 Login
Als Studierende:r  
möchte ich mich anmelden können,  
damit ich Zugriff auf meine Kurse und Aufgaben habe.

### US-03 Logout
Als Studierende:r  
möchte ich mich abmelden können,  
damit niemand anderes Zugriff auf meine Daten hat.

---

## Epic: Kursverwaltung

### US-04 Kurs erstellen
Als Studierende:r  
möchte ich neue Kurse anlegen können,  
damit ich Aufgaben organisieren kann.

### US-05 Kurs bearbeiten
Als Studierende:r  
möchte ich Kursinformationen ändern können,  
damit meine Daten aktuell bleiben.

### US-06 Kurs löschen
Als Studierende:r  
möchte ich nicht mehr benötigte Kurse löschen können,  
damit meine Übersicht sauber bleibt.

---

## Epic: Aufgabenverwaltung

### US-07 Aufgabe erstellen
Als Studierende:r  
möchte ich Aufgaben hinzufügen können,  
damit ich keine Abgaben vergesse.

### US-08 Aufgabe bearbeiten
Als Studierende:r  
möchte ich Aufgaben aktualisieren können,  
damit Informationen korrekt bleiben.

### US-09 Aufgabe löschen
Als Studierende:r  
möchte ich Aufgaben entfernen können,  
damit erledigte oder falsche Einträge verschwinden.

### US-10 Aufgabenstatus ändern
Als Studierende:r  
möchte ich Aufgaben als erledigt markieren können,  
damit ich meinen Fortschritt sehe.

### US-11 Aufgaben filtern
Als Studierende:r  
möchte ich Aufgaben nach Kurs oder Deadline filtern können,  
damit ich wichtige Aufgaben schneller finde.

---

## Epic: Benachrichtigungen

### US-12 Erinnerungen erhalten
Als Studierende:r  
möchte ich Erinnerungen vor Abgabeterminen erhalten,  
damit ich keine Deadline verpasse.

### US-13 Dringende Aufgaben erkennen
Als Studierende:r  
möchte ich bald fällige Aufgaben hervorgehoben sehen,  
damit ich Prioritäten setzen kann.

---

# 5. Akzeptanzkriterien (Beispiele)

## AC-01 Aufgabe erstellen
- Eine Aufgabe muss einen Titel besitzen.
- Eine Aufgabe muss einem Kurs zugeordnet sein.
- Nach dem Speichern erscheint die Aufgabe in der Aufgabenliste.

## AC-02 Aufgabe abschließen
- Benutzer:innen können den Status auf „Erledigt“ setzen.
- Erledigte Aufgaben werden visuell markiert.

## AC-03 Erinnerungen
- Die App sendet spätestens 24 Stunden vor einer Deadline eine Erinnerung.

---

# 6. Mögliche Erweiterungen

- Kalenderintegration
- Datei-Uploads für Aufgaben
- Gruppenprojekte
- Synchronisation mit Uni-Plattformen
- Dark Mode
- Push-Benachrichtigungen
- KI-basierte Priorisierung von Aufgaben
