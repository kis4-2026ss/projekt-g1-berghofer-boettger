# Gemini Ergebnis: Student Task Manager - Structured Prompt

## Verwendeter Prompt

Erstelle Requirements und User Stories für eine einfache App, mit der Studierende Aufgaben für verschiedene Kurse verwalten können.

Berücksichtige dabei:

- funktionale Requirements
- nicht-funktionale Requirements
- User Stories im Format: Als Student möchte ich ..., damit ...
- eine klare und übersichtliche Struktur

## Ergebnis

# Requirements und User Stories: Studierenden-Aufgabenplaner (StudyTask App)

Dieses Dokument beschreibt die funktionalen und nicht-funktionalen Anforderungen sowie die User Stories für eine einfache mobile/Web-Anwendung, mit der Studierende ihre Aufgaben für verschiedene Kurse verwalten können.

---

## 1. Einleitung und Zielsetzung
Ziel der App ist es, Studierenden ein einfaches, intuitives Werkzeug an die Hand zu geben, um den Überblick über Abgabefristen, Hausaufgaben und Projektarbeiten in verschiedenen Kursen (Modulen) zu behalten. Die App soll den akademischen Alltag strukturieren und das Risko von verpassten Deadlines minimieren.

---

## 2. Funktionale Requirements (FR)

Die funktionalen Anforderungen beschreiben die spezifischen Funktionen und Verhaltensweisen, die das System bereitstellen muss.

### FR1: Kursverwaltung
* **FR1.1:** Das System muss es dem Nutzer ermöglichen, Kurse (z. B. "Mathematik 1", "Software Engineering") zu erstellen.
* **FR1.2:** Jeder Kurs muss mindestens einen Namen und optional eine Farbcodierung zur visuellen Trennung besitzen.
* **FR1.3:** Nutzer müssen bestehende Kurse bearbeiten und löschen können. Das Löschen eines Kurses kaskadiert auf alle darin enthaltenen Aufgaben (nach Bestätigung).

### FR2: Aufgabenverwaltung (To-Dos)
* **FR2.1:** Das System muss es dem Nutzer ermöglichen, Aufgaben zu erstellen und einem spezifischen Kurs zuzuordnen.
* **FR2.2:** Eine Aufgabe muss folgende Datenfelder enthalten:
    * Titel (Pflichtfeld)
    * Beschreibung (Optional)
    * Fälligkeitsdatum / Deadline (Pflichtfeld)
    * Status (z. B. "Offen", "In Bearbeitung", "Erledigt")
    * Priorität (z. B. "Niedrig", "Mittel", "Hoch")
* **FR2.3:** Nutzer müssen Aufgaben als "Erledigt" markieren können, ohne die Aufgabe komplett löschen zu müssen.
* **FR2.4:** Aufgaben müssen bearbeitet und gelöscht werden können.

### FR3: Dashboard und Filterung
* **FR3.1:** Die Startseite (Dashboard) muss eine chronologische Übersicht aller anstehenden Aufgaben (sortiert nach dem nächsten Fälligkeitsdatum) anzeigen.
* **FR3.2:** Das System muss eine Filterfunktion nach Kursen bereitstellen.
* **FR3.3:** Das System muss eine Filterfunktion nach Status (z. B. "Nur offene Aufgaben anzeigen") bereitstellen.

### FR4: Benachrichtigungen (Erinnerungen)
* **FR4.1:** Das System muss den Nutzer standardmäßig 24 Stunden vor Ablauf einer Deadline an eine offene Aufgabe erinnern.
* **FR4.2:** Der Nutzer muss die Erinnerungszeit für eine Aufgabe individuell anpassen können (z. B. 2 Stunden vorher, 3 Tage vorher).

---

## 3. Nicht-funktionale Requirements (NFR)

Die nicht-funktionalen Anforderungen definieren Qualitätsmerkmale, Rahmenbedingungen und technische Einschränkungen des Systems.

### NFR1: Benutzbarkeit (Usability)
* **NFR1.1:** Die Benutzeroberfläche (UI) muss intuitiv und mit minimalem Schulungsaufwand bedienbar sein. Das Anlegen einer Aufgabe darf nicht mehr als drei Klicks/Taps erfordern.
* **NFR1.2:** Die Anwendung muss responsiv sein und sowohl auf Smartphones (iOS/Android) als auch auf Desktop-Browsern optimal dargestellt werden.

### NFR2: Leistung und Skalierbarkeit (Performance)
* **NFR2.1:** Die Ladezeit des Dashboards darf bei einer durchschnittlichen Internetverbindung und bis zu 100 aktiven Aufgaben 1,5 Sekunden nicht überschreiten.
* **NFR2.2:** Statusänderungen von Aufgaben (z. B. als "Erledigt" markieren) müssen innerhalb von 200 Millisekunden visuell auf der UI reflektiert werden.

### NFR3: Zuverlässigkeit und Datenhaltung (Reliability & Storage)
* **NFR3.1:** Eingegebene Daten müssen persistent in einer Datenbank gespeichert werden, sodass sie auch nach dem Schließen der App oder bei einem Neustart des Geräts vollständig erhalten bleiben.
* **NFR3.2:** Die App muss grundlegende Offline-Funktionalitäten unterstützen: Bereits geladene Aufgaben müssen offline sichtbar sein, und offline vorgenommene Änderungen müssen synchronisiert werden, sobald wieder eine Internetverbindung besteht.

### NFR4: Sicherheit und Datenschutz (Security)
* **NFR4.1:** Die Authentifizierung der Nutzer muss über ein sicheres Login-Verfahren (E-Mail/Passwort oder OAuth wie Google/Apple) erfolgen.
* **NFR4.2:** Alle Datenübertragungen zwischen dem Client und dem Server müssen via HTTPS verschlüsselt sein.

---

## 4. User Stories

Die User Stories beschreiben die Anforderungen aus Sicht der Endanwender (Studierenden) im standardisierten Format.

### Epics / Themenbereich: Kurs-Setup
* **US1.1:** **Als** Student **möchte ich** neue Kurse mit individuellen Namen und Farben anlegen, **damit** ich meine Aufgaben visuell nach Fächern trennen und strukturieren kann.
* **US1.2:** **Als** Student **möchte ich** bestehende Kurse umbenennen oder löschen können, **damit** meine Kursliste aktuell bleibt, wenn sich mein Stundenplan ändert.

### Epics / Themenbereich: Aufgaben-Alltag
* **US2.1:** **Als** Student **möchte ich** schnell eine neue Aufgabe mit einem Titel und einer Deadline erstellen und einem Kurs zuweisen, **damit** ich sie im Vorlesungstrubel nicht vergesse.
* **US2.2:** **Als** Student **möchte ich** einer Aufgabe Notizen und eine Priorität hinzufügen können, **damit** ich weiß, worum es genau geht und welche Aufgaben am wichtigsten sind.
* **US2.3:** **Als** Student **möchte ich** eine Aufgabe mit einem einzigen Klick als "Erledigt" markieren können, **damit** sie aus meiner aktuellen To-Do-Liste verschwindet und ich ein Erfolgserlebnis habe.
* **US2.4:** **Als** Student **möchte ich** erledigte Aufgaben in einer Historie einsehen können, **damit** ich am Ende des Semesters nachvollziehen kann, was ich alles geleistet habe.

### Epics / Themenbereich: Übersicht & Zeitmanagement
* **US3.1:** **Als** Student **möchte ich** beim Öffnen der App sofort alle chronologisch kritischen Deadlines sehen, **damit** ich sofort weiß, was ich als Nächstes tun muss.
* **US3.2:** **Als** Student **möchte ich** meine Aufgabenliste nach einem bestimmten Kurs filtern können, **damit** ich mich gezielt auf die Vorbereitung für dieses eine Fach konzentrieren kann.
* **US3.3:** **Als** Student **möchte ich** Push-Benachrichtigungen auf mein Handy bekommen, bevor eine Deadline abläuft, **damit** ich auch bei stressigen Phasen keine Abgabe verpasse.
