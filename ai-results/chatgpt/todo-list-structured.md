# ChatGPT Ergebnis: Simple To-do List - Simple Prompt

## Verwendeter Prompt

Erstelle Requirements und User Stories für eine einfache To-do-Listen-App.

## Ergebnis

# To-do-Listen-App

## 1. Projektübersicht

Die Anwendung ermöglicht Benutzern das einfache Verwalten von Aufgaben (To-dos).
Ziel ist eine minimalistische, intuitive und schnelle To-do-Listen-App für den täglichen Gebrauch.

---

# 2. Funktionale Anforderungen (Functional Requirements)

## FR-1 Aufgaben erstellen
Der Benutzer kann neue Aufgaben anlegen.

### Akzeptanzkriterien
- Ein Eingabefeld für den Titel ist vorhanden.
- Eine Aufgabe kann durch Klick auf „Hinzufügen“ erstellt werden.
- Leere Aufgaben dürfen nicht gespeichert werden.

---

## FR-2 Aufgaben anzeigen
Der Benutzer kann alle vorhandenen Aufgaben sehen.

### Akzeptanzkriterien
- Aufgaben werden in einer Liste dargestellt.
- Jede Aufgabe zeigt mindestens:
  - Titel
  - Status (offen/erledigt)

---

## FR-3 Aufgaben als erledigt markieren
Der Benutzer kann Aufgaben als erledigt markieren.

### Akzeptanzkriterien
- Eine Checkbox oder Schaltfläche ist vorhanden.
- Erledigte Aufgaben werden visuell gekennzeichnet.

---

## FR-4 Aufgaben bearbeiten
Der Benutzer kann bestehende Aufgaben ändern.

### Akzeptanzkriterien
- Der Titel einer Aufgabe kann angepasst werden.
- Änderungen werden sofort gespeichert.

---

## FR-5 Aufgaben löschen
Der Benutzer kann Aufgaben entfernen.

### Akzeptanzkriterien
- Jede Aufgabe besitzt eine Löschfunktion.
- Gelöschte Aufgaben verschwinden sofort aus der Liste.

---

## FR-6 Aufgaben filtern
Der Benutzer kann Aufgaben nach Status filtern.

### Akzeptanzkriterien
- Filteroptionen:
  - Alle
  - Offen
  - Erledigt
- Die Liste aktualisiert sich entsprechend.

---

## FR-7 Daten lokal speichern
Die Aufgaben bleiben nach dem Neuladen der Seite erhalten.

### Akzeptanzkriterien
- Speicherung erfolgt lokal im Browser (z. B. Local Storage).
- Nach erneutem Öffnen der App sind die Aufgaben weiterhin vorhanden.

---

# 3. Nichtfunktionale Anforderungen (Non-Functional Requirements)

## NFR-1 Benutzerfreundlichkeit
- Die Oberfläche soll einfach und intuitiv bedienbar sein.
- Neue Benutzer sollen die App ohne Anleitung verstehen.

## NFR-2 Performance
- Aufgaben sollen ohne merkbare Verzögerung gespeichert und angezeigt werden.

## NFR-3 Responsives Design
- Die Anwendung soll auf Desktop und Mobilgeräten nutzbar sein.

## NFR-4 Verfügbarkeit
- Die App soll vollständig im Browser funktionieren.

## NFR-5 Wartbarkeit
- Der Code soll modular und gut dokumentiert sein.

---

# 4. User Stories

## US-1 Aufgabe erstellen
**Als** Benutzer  
**möchte ich** neue Aufgaben hinzufügen  
**damit** ich meine Aufgaben organisieren kann.

### Akzeptanzkriterien
- Eingabe eines Aufgabentitels möglich
- Aufgabe erscheint direkt in der Liste

---

## US-2 Aufgabe erledigen
**Als** Benutzer  
**möchte ich** Aufgaben als erledigt markieren  
**damit** ich meinen Fortschritt sehen kann.

### Akzeptanzkriterien
- Aufgabe kann per Checkbox markiert werden
- Erledigte Aufgaben werden optisch hervorgehoben

---

## US-3 Aufgabe bearbeiten
**Als** Benutzer  
**möchte ich** Aufgaben bearbeiten  
**damit** ich Änderungen an meinen Aufgaben vornehmen kann.

### Akzeptanzkriterien
- Titel kann geändert werden
- Änderungen bleiben gespeichert

---

## US-4 Aufgabe löschen
**Als** Benutzer  
**möchte ich** Aufgaben löschen  
**damit** ich nicht mehr benötigte Aufgaben entfernen kann.

### Akzeptanzkriterien
- Aufgabe kann gelöscht werden
- Liste wird sofort aktualisiert

---

## US-5 Aufgaben filtern
**Als** Benutzer  
**möchte ich** Aufgaben nach Status filtern  
**damit** ich mich auf offene oder erledigte Aufgaben konzentrieren kann.

### Akzeptanzkriterien
- Filter „Alle“, „Offen“, „Erledigt“ vorhanden
- Anzeige aktualisiert sich korrekt

---

## US-6 Daten behalten
**Als** Benutzer  
**möchte ich** dass meine Aufgaben gespeichert bleiben  
**damit** ich sie nach dem Neuladen nicht erneut eingeben muss.

### Akzeptanzkriterien
- Aufgaben bleiben nach Browser-Neustart erhalten

---

# 5. Technische Empfehlungen

## Frontend
- HTML5
- CSS3
- JavaScript (Vanilla JS oder Framework wie React)

## Datenspeicherung
- Browser Local Storage

## Optional Erweiterbar
- Benutzerkonten
- Cloud-Synchronisierung
- Erinnerungen
- Kategorien & Prioritäten
- Dark Mode

---

# 6. MVP (Minimum Viable Product)

Das MVP umfasst:
- Aufgaben erstellen
- Aufgaben anzeigen
- Aufgaben erledigen
- Aufgaben löschen
- Lokale Speicherung
