# Gemini Ergebnis: Student Task Manager - Simple Prompt

## Verwendeter Prompt

Erstelle Requirements und User Stories für eine einfache App, mit der Studierende Aufgaben für verschiedene Kurse verwalten können.

## Ergebnis

# Software Requirements Specification (SRS) & User Stories: StudiTask App
**Projekt:** Einfache App zur Aufgabenverwaltung für Studierende  
**Format:** Markdown (.md)  
**Version:** 1.0  
**Datum:** 24. Mai 2026  

---

## 1. Einleitung & Zielsetzung
Die **StudiTask App** ist eine schlanke, intuitive Anwendung, die speziell für Studierende entwickelt wird, um ihren akademischen Alltag zu strukturieren. Studierende stehen oft vor der Herausforderung, Abgabefristen, Projektarbeiten und Prüfungstermine über mehrere Kurse hinweg parallel zu koordinieren. 

Ziel dieser App ist es, eine zentrale Plattform zu bieten, auf der Nutzer Kurse anlegen, Aufgaben mit Fristen erfassen und ihren Bearbeitungsstatus visuell nachverfolgen können. Der Fokus liegt auf Einfachheit, schneller Bedienbarkeit und einer klaren Übersicht.

---

## 2. Systemanforderungen (Anforderungskatalog)

### 2.1 Funktionale Anforderungen (FR)

| ID | Komponente | Beschreibung | Priorität |
| :--- | :--- | :--- | :--- |
| **FR-100** | **Kursverwaltung** | Das System muss es dem Nutzer erlauben, Kurse mit einem Namen und einer optionalen Farbe (zur visuellen Kennzeichnung) zu erstellen. | Hoch (Must-have) |
| **FR-101** | **Kursverwaltung** | Das System muss es erlauben, bestehende Kurse zu bearbeiten oder zu löschen. Beim Löschen eines Kurses werden alle zugeordneten Aufgaben ebenfalls gelöscht (Kaskadierung). | Hoch (Must-have) |
| **FR-200** | **Aufgabenverwaltung** | Das System muss es erlauben, Aufgaben zu erstellen. Eine Aufgabe besteht aus: Titel, Beschreibung (optional), Fälligkeitsdatum (Deadline), Priorität (Niedrig, Mittel, Hoch) und Kurszuordnung. | Hoch (Must-have) |
| **FR-201** | **Aufgabenverwaltung** | Das System muss es dem Nutzer ermöglichen, Aufgaben als "Offen", "In Bearbeitung" oder "Erledigt" zu markieren. | Hoch (Must-have) |
| **FR-202** | **Aufgabenverwaltung** | Der Nutzer muss bestehende Aufgaben bearbeiten und unwiderruflich löschen können. | Hoch (Must-have) |
| **FR-300** | **Dashboard / Ansichten** | Das System muss eine chronologische Übersicht aller anstehenden Aufgaben bereitstellen, sortiert nach dem Fälligkeitsdatum (nächste Deadlines zuerst). | Hoch (Must-have) |
| **FR-301** | **Dashboard / Ansichten** | Das System muss eine Filterfunktion nach Kursen sowie nach dem Status der Aufgaben (z. B. "nur offene anzeigen") bereitstellen. | Mittel (Should-have) |
| **FR-400** | **Benachrichtigungen** | Das System sollte den Nutzer 24 Stunden vor Ablauf einer Aufgaben-Deadline per Push-Benachrichtigung oder In-App-Hinweis erinnern. | Mittel (Should-have) |

### 2.2 Nicht-funktionale Anforderungen (NFR)

| ID | Kategorie | Beschreibung | Priorität |
| :--- | :--- | :--- | :--- |
| **NFR-1** | **Usability (Bedienbarkeit)** | Die App muss ohne Schulung oder Handbuch intuitiv bedienbar sein. Das Erstellen einer Aufgabe darf nicht mehr als drei Klicks/Taps erfordern. | Hoch |
| **NFR-2** | **Performance (Leistung)** | Die Ladezeit beim Öffnen der App oder beim Wechseln zwischen Kursansichten muss unter 1 Sekunde liegen. | Hoch |
| **NFR-3** | **Verfügbarkeit** | Die App muss lokal auf dem Gerät des Nutzers auch ohne aktive Internetverbindung (Offline-Modus) voll funktionsfähig sein. | Hoch |
| **NFR-4** | **Plattformkonformität** | Die Benutzeroberfläche muss responsiv sein und sich sowohl auf Smartphones (iOS/Android) als auch im Web-Browser korrekt darstellen. | Mittel |

---

## 3. User Stories & Akzeptanzkriterien

Die folgenden User Stories beschreiben die Anforderungen aus der Perspektive der Studierenden (Endnutzer).

### Epic 1: Kursorganisation
Zentrale Verwaltung der universitären Module/Kurse.

#### User Story US-1.1: Kurs anlegen
> **Als** Studierender  
> **möchte ich** neue Kurse mit einem Namen und einer Farbe anlegen können,  
> **sodass ich** meine Aufgaben später visuell nach Fächern trennen kann.

* **Akzeptanzkriterien:**
    * [ ] Es gibt eine Schaltfläche "Kurs hinzufügen".
    * [ ] Das Feld "Kursname" ist ein Pflichtfeld (min. 3, max. 50 Zeichen).
    * [ ] Der Nutzer kann aus einer vordefinierten Farbpalette (mind. 6 Farben) eine Farbe wählen.
    * [ ] Nach dem Speichern ist der Kurs sofort in der Kursliste sichtbar.
    * [ ] Doppelte Kursnamen für denselben Nutzer werden mit einer Fehlermeldung abgelehnt.

#### User Story US-1.2: Kurs löschen
> **Als** Studierender  
> **möchte ich** einen Kurs löschen können,  
> **sodass** meine Übersicht nach Semesterende aufgeräumt bleibt.

* **Akzeptanzkriterien:**
    * [ ] In der Kursübersicht oder den Kurseinstellungen existiert eine "Löschen"-Option.
    * [ ] Vor dem endgültigen Löschen erscheint ein Warnhinweis: *"Möchten Sie diesen Kurs und alle darin enthaltenen Aufgaben wirklich löschen?"*.
    * [ ] Bestätigt der Nutzer, wird der Kurs mitsamt allen zugeordneten Aufgaben permanent gelöscht.

---

### Epic 2: Aufgabenmanagement
Erfassung und Pflege der täglichen To-Dos.

#### User Story US-2.1: Aufgabe erstellen
> **Als** Studierender  
> **möchte ich** eine neue Aufgabe für einen bestimmten Kurs eintragen,  
> **sodass ich** keine Hausaufgabe oder Projektarbeit vergesse.

* **Akzeptanzkriterien:**
    * [ ] Es gibt ein Formular mit den Feldern: Titel (Pflichtfeld), Beschreibung (optional), Fälligkeitsdatum (Pflichtfeld), Priorität (Dropdown: Niedrig, Mittel, Hoch) und Kursauswahl (Dropdown der erstellten Kurse).
    * [ ] Das Fälligkeitsdatum darf standardmäßig nicht in der Vergangenheit liegen.
    * [ ] Die Aufgabe wird nach dem Speichern mit dem Status "Offen" initialisiert.

#### User Story US-2.2: Aufgabenstatus aktualisieren
> **Als** Studierender  
> **möchte ich** den Status einer Aufgabe von "Offen" auf "In Bearbeitung" oder "Erledigt" setzen können,  
> **sodass ich** meinen aktuellen Fortschritt jederzeit im Blick habe.

* **Akzeptanzkriterien:**
    * [ ] Direkt in der Aufgabenliste gibt es eine Schnellauswahl (z. B. eine Checkbox oder ein Status-Icon), um eine Aufgabe als "Erledigt" zu markieren.
    * [ ] Erledigte Aufgaben werden visuell ausgegraut oder durchgestrichen dargestellt.
    * [ ] Der Status kann in den Aufgabendetails jederzeit wieder zurück auf "Offen" oder "In Bearbeitung" geändert werden.

---

### Epic 3: Übersicht & Filter
Schnelles Wiederfinden und Priorisieren von Aufgaben.

#### User Story US-3.1: Chronologisches Dashboard (Deadline-Ansicht)
> **Als** Studierender  
> **möchte ich** alle anstehenden Aufgaben sortiert nach ihrer Deadline sehen,  
> **sodass ich** sofort weiß, welche Aufgabe als nächstes fällig ist.

* **Akzeptanzkriterien:**
    * [ ] Die Startseite der App zeigt eine Liste aller nicht-erledigten Aufgaben.
    * [ ] Die Sortierung erfolgt aufsteigend nach dem Fälligkeitsdatum (wichtigste/nächste Deadline ganz oben).
    * [ ] Aufgaben, deren Deadline überschritten ist und die nicht "Erledigt" sind, werden rot hervorgehoben.

#### User Story US-3.2: Filtern nach Kurs
> **Als** Studierender  
> **möchte ich** meine Aufgabenliste nach einem bestimmten Kurs filtern können,  
> **sodass ich** mich gezielt auf die Aufgaben für ein einzelnes Fach konzentrieren kann.

* **Akzeptanzkriterien:**
    * [ ] Am oberen Bildschirmrand der Aufgabenübersicht befindet sich eine Filter-Leiste mit allen angelegten Kursen (sowie einer Option "Alle Kurse").
    * [ ] Beim Klick auf einen Kurs werden sofort nur noch die Aufgaben geladen, die diesem Kurs zugeordnet sind.
    * [ ] Die Filterung erfolgt ohne spürbare Verzögerung (< 200ms).
