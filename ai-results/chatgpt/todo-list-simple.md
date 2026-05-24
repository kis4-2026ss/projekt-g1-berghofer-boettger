# ChatGPT Ergebnis: Simple To-do List - Simple Prompt

## Verwendeter Prompt

Erstelle Requirements und User Stories für eine einfache To-do-Listen-App.

## Ergebnis

# To-do-Listen-App

## 1. Projektübersicht

Die Anwendung ist eine einfache To-do-Listen-App, mit der Benutzer Aufgaben erstellen, verwalten und als erledigt markieren können.  
Ziel ist eine intuitive und minimalistische Anwendung für den täglichen Gebrauch.

---

# 2. Funktionale Requirements

## 2.1 Aufgaben verwalten

### FR-001 – Aufgabe erstellen
Der Benutzer kann eine neue Aufgabe hinzufügen.

**Akzeptanzkriterien**
- Eingabefeld für Titel vorhanden
- Aufgabe wird nach dem Speichern angezeigt
- Leere Aufgaben dürfen nicht gespeichert werden

---

### FR-002 – Aufgabe anzeigen
Der Benutzer kann alle vorhandenen Aufgaben sehen.

**Akzeptanzkriterien**
- Aufgaben werden in einer Liste dargestellt
- Jede Aufgabe zeigt Titel und Status an

---

### FR-003 – Aufgabe als erledigt markieren
Der Benutzer kann Aufgaben als erledigt markieren.

**Akzeptanzkriterien**
- Checkbox oder Button vorhanden
- Erledigte Aufgaben werden visuell hervorgehoben
- Status bleibt nach Aktualisierung erhalten

---

### FR-004 – Aufgabe bearbeiten
Der Benutzer kann bestehende Aufgaben bearbeiten.

**Akzeptanzkriterien**
- Titel kann geändert werden
- Änderungen werden gespeichert

---

### FR-005 – Aufgabe löschen
Der Benutzer kann Aufgaben entfernen.

**Akzeptanzkriterien**
- Löschfunktion vorhanden
- Aufgabe verschwindet sofort aus der Liste

---

## 2.2 Filterfunktionen

### FR-006 – Aufgaben filtern
Der Benutzer kann Aufgaben nach Status filtern.

**Akzeptanzkriterien**
- Filter für:
  - Alle
  - Offen
  - Erledigt
- Liste aktualisiert sich entsprechend

---

# 3. Nicht-funktionale Requirements

## NFR-001 – Benutzerfreundlichkeit
Die Anwendung soll einfach und intuitiv bedienbar sein.

---

## NFR-002 – Performance
Aktionen wie Hinzufügen oder Löschen sollen ohne merkliche Verzögerung erfolgen.

---

## NFR-003 – Responsives Design
Die Anwendung soll auf Desktop und Mobilgeräten nutzbar sein.

---

## NFR-004 – Datenspeicherung
Aufgaben sollen lokal gespeichert bleiben (z. B. Local Storage).

---

# 4. User Stories

---

## US-001 – Aufgabe erstellen

**Als** Benutzer  
**möchte ich** neue Aufgaben hinzufügen  
**damit** ich meine Aufgaben festhalten kann.

### Akzeptanzkriterien
- Aufgabe kann eingegeben werden
- Aufgabe erscheint in der Liste
- Leere Eingaben sind nicht erlaubt

---

## US-002 – Aufgaben ansehen

**Als** Benutzer  
**möchte ich** alle meine Aufgaben sehen  
**damit** ich einen Überblick habe.

### Akzeptanzkriterien
- Alle Aufgaben werden angezeigt
- Status jeder Aufgabe ist sichtbar

---

## US-003 – Aufgabe erledigen

**Als** Benutzer  
**möchte ich** Aufgaben als erledigt markieren  
**damit** ich abgeschlossene Aufgaben erkennen kann.

### Akzeptanzkriterien
- Aufgabe kann markiert werden
- Erledigte Aufgaben sind optisch unterscheidbar

---

## US-004 – Aufgabe bearbeiten

**Als** Benutzer  
**möchte ich** Aufgaben bearbeiten  
**damit** ich Änderungen vornehmen kann.

### Akzeptanzkriterien
- Titel kann geändert werden
- Änderungen werden gespeichert

---

## US-005 – Aufgabe löschen

**Als** Benutzer  
**möchte ich** Aufgaben löschen  
**damit** ich nicht mehr benötigte Aufgaben entfernen kann.

### Akzeptanzkriterien
- Aufgabe kann gelöscht werden
- Liste aktualisiert sich sofort

---

## US-006 – Aufgaben filtern

**Als** Benutzer  
**möchte ich** Aufgaben nach Status filtern  
**damit** ich mich auf relevante Aufgaben konzentrieren kann.

### Akzeptanzkriterien
- Filteroptionen vorhanden
- Gefilterte Ergebnisse werden korrekt angezeigt

---

# 5. MVP-Umfang

Die erste Version (MVP) enthält:

- Aufgaben erstellen
- Aufgaben anzeigen
- Aufgaben als erledigt markieren
- Aufgaben löschen
- Lokale Datenspeicherung

Nicht im MVP:
- Benutzerkonten
- Cloud-Synchronisation
- Erinnerungen
- Kategorien oder Prioritäten

---

# 6. Technische Empfehlungen

## Frontend
- HTML
- CSS
- JavaScript
- Optional: React oder Vue

## Speicherung
- Browser Local Storage

## Deployment
- GitHub Pages oder Vercel

---