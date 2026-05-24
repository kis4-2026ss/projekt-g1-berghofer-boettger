# Gemini Ergebnis: Student Task Manager - Iterative Prompt

## Verwendete Prompts

### Prompt 1

Erstelle Requirements und User Stories für eine einfache App, mit der Studierende Aufgaben für verschiedene Kurse verwalten können.

### Prompt 2

Überarbeite das Ergebnis und ergänze fehlende funktionale und nicht-funktionale Requirements.

### Prompt 3

Verbessere die User Stories und achte darauf, dass sie im Format „Als Student möchte ich ..., damit ...“ geschrieben sind.

## Ergebnis

# Requirements und User Stories: Studenten-Aufgaben-Manager (TaskStudent App) - Optimierte Version

Dieses Dokument enthält die funktionalen und nicht-funktionalen Anforderungen sowie die User Stories für eine mobile/Web-Applikation, mit der Studierende ihre akademischen Aufgaben und Fristen kursbasiert verwalten können.

---

## 1. Produktvision & Zielsetzung
Die App **TaskStudent** hilft Studierenden dabei, ihren akademischen Alltag zu strukturieren. Da Aufgaben und Fristen über verschiedene Kurse und Plattformen hinweg anfallen, bietet diese App eine zentrale, intuitive Oberfläche. Ziel ist es, Aufgaben nach Kursen zu sortieren, Fristen über smarte Erinnerungen zu überwachen und den Bearbeitungsstatus transparent zu verfolgen.

---

## 2. Funktionale Anforderungen (Functional Requirements)

### 2.1 Benutzerverwaltung & Synchronisation
- **FR-1:** Das System muss es Benutzern erlauben, ein Konto zu erstellen (Registrierung per E-Mail/Passwort oder OAuth wie Google/Apple).
- **FR-2:** Das System muss die Daten des Benutzers sicher in der Cloud synchronisieren, damit eine plattformübergreifende Nutzung (Web & Mobile) möglich ist.
- **FR-3:** Das System muss eine "Passwort zurücksetzen"-Funktion bereitstellen.

### 2.2 Kursverwaltung (Course Management)
- **FR-4:** Das System muss es dem Benutzer erlauben, neue Kurse (z. B. "Mathematik 1") zu erstellen.
- **FR-5:** Jeder Kurs muss einen eindeutigen Namen, ein optionales Semester (z. B. "WiSe 2026") und eine optionale Farbe zur visuellen Codierung besitzen.
- **FR-6:** Das System muss es erlauben, bestehende Kurse zu bearbeiten, zu löschen oder zu archivieren.
- **FR-7:** Beim Archivieren eines Kurses werden alle zugehörigen Aufgaben standardmäßig aus der aktiven Ansicht ausgeblendet, bleiben aber in der Historie erhalten.

### 2.3 Aufgabenverwaltung (Task Management)
- **FR-8:** Das System muss es dem Benutzer erlauben, Aufgaben zu erstellen und einem spezifischen Kurs zuzuordnen.
- **FR-9:** Eine Aufgabe muss folgende Datenfelder enthalten:
  - Titel (Pflichtfeld, max. 100 Zeichen)
  - Beschreibung (Optional, Rich-Text oder Markdown-Unterstützung)
  - Fälligkeitsdatum (Deadline) und Uhrzeit (Pflichtfeld für die Kalenderansicht)
  - Status (*Offen*, *In Bearbeitung*, *Erledigt*)
  - Priorität (*Niedrig*, *Mittel*, *Hoch*)
- **FR-10:** Der Benutzer muss den Status einer Aufgabe per Checkbox oder Drag-and-Drop direkt in der Listenansicht ändern können.
- **FR-11:** Das System muss das Anhängen von Unteraufgaben (Checklisten) innerhalb einer Hauptaufgabe erlauben.

### 2.4 Benachrichtigungen & Erinnerungen
- **FR-12:** Das System muss automatische Erinnerungen (Push-Benachrichtigungen oder E-Mail) für anstehende Deadlines senden.
- **FR-13:** Der Benutzer muss die Erinnerungszeitpunkte individuell pro Aufgabe oder global einstellen können (z. B. 24 Stunden vorher, 2 Stunden vorher).

### 2.5 Dashboard, Kalender & Filter
- **FR-14:** Das System muss ein Dashboard mit einer chronologischen Liste ("Dringendste zuerst") anzeigen.
- **FR-15:** Das System muss eine Kalenderansicht (Monats- und Wochenansicht) bereitstellen, in der Aufgaben als Termine visualisiert werden.
- **FR-16:** Das System muss Filter nach Kurs, Status, Priorität und Zeitraum (z. B. "Diese Woche") sowie eine Volltextsuche unterstützen.

---

## 3. Nicht-funktionale Anforderungen (Non-Functional Requirements)

### 3.1 Usability & Barrierefreiheit
- **NFR-1 (Einfachheit):** Die Erstellung einer Aufgabe darf vom Startbildschirm aus nicht mehr als 3 Interaktionen (Klicks/Taps) erfordern.
- **NFR-2 (Barrierefreiheit / Accessibility):** Die App muss den WCAG 2.1 AA-Richtlinien entsprechen (z. B. ausreichender Farbkontrast für die Kursfarben, Screenreader-Unterstützung).
- **NFR-3 (Responsive Design):** Die UI muss für Displays von 4 Zoll (Smartphone) bis zu 4K-Monitoren optimiert sein. Dark Mode muss unterstützt werden.

### 3.2 Performance & Zuverlässigkeit
- **NFR-4 (Offline-First):** Die App muss vollständig offline funktionsfähig sein. Alle Datenänderungen werden lokal gecached und bei bestehender Verbindung konfliktfrei mit der Cloud synchronisiert.
- **NFR-5 (Ladezeit & Performance):** Die Interaktionslatenz (z. B. Abhaken einer Aufgabe) muss unter 100ms liegen. Das Laden des Dashboards darf bei stabiler Verbindung nicht länger als 1 Sekunde dauern.

### 3.3 Sicherheit & Datenschutz
- **NFR-6 (DSGVO):** Alle personenbezogenen Daten müssen DSGVO-konform verarbeitet werden. Der Benutzer muss sein Konto und alle damit verbundenen Daten unwiderruflich selbst löschen können.
- **NFR-7 (Verschlüsselung):** Die Datenübertragung muss via HTTPS/TLS 1.3 verschlüsselt sein. Passwörter müssen gesalzen und gehasht (z. B. mit bcrypt) gespeichert werden.

---

## 4. User Stories

### Epic 1: Account & Synchronisation

#### US-1.1: Registrierung und Login
- **User Story:** Als Student möchte ich mich mit meiner universitären E-Mail-Adresse registrieren, damit meine Aufgaben zwischen all meinen Geräten synchronisiert werden.
- **Akzeptanzkriterien:**
  1. Registrierungsformular validiert die E-Mail-Adresse und fordert ein sicheres Passwort (min. 8 Zeichen, 1 Sonderzeichen).
  2. Nach der Registrierung wird eine Bestätigungs-E-Mail versendet.
  3. Ein Login via "Sign in with Google/Apple" ist auf der Startseite integriert.

---

### Epic 2: Kursorganisation

#### US-2.1: Kurs anlegen
- **User Story:** Als Student möchte ich neue Kurse mit einem Namen und einer spezifischen Farbe anlegen, damit ich meine Aufgaben visuell sofort dem richtigen Fach zuordnen kann.
- **Akzeptanzkriterien:**
  1. Ein "Kurs hinzufügen"-Dialog erlaubt die Eingabe eines Namens (Pflicht) und die Auswahl eines Semesters.
  2. Es steht eine Palette aus 12 kontrastreichen Farben zur Auswahl.
  3. Die gewählte Farbe wird als Indikator bei allen zugehörigen Aufgaben angezeigt.

#### US-2.2: Kurs archivieren
- **User Story:** Als Student möchte ich alte oder abgeschlossene Kurse archivieren, damit meine aktive Kursübersicht übersichtlich bleibt.
- **Akzeptanzkriterien:**
  1. In den Kurseinstellungen gibt es die Option "Kurs archivieren".
  2. Archivierte Kurse tauchen nicht mehr in den aktiven Filterleisten auf.
  3. In einem separaten Bereich "Archiv" können diese Kurse eingesehen und reaktiviert werden.

---

### Epic 3: Aufgaben- & Subtask-Verwaltung

#### US-3.1: Aufgabe erstellen
- **User Story:** Als Student möchte ich eine neue Aufgabe mit einer Beschreibung, einer Deadline und einer Priorität erstellen, damit ich meine anstehenden Abgaben präzise planen kann.
- **Akzeptanzkriterien:**
  1. Das Erstellungsformular bietet optionale Felder für Beschreibung (Textarea) und ein Dropdown für Priorität (Niedrig, Mittel, Hoch).
  2. Es gibt ein Pflichtfeld für das Fälligkeitsdatum inklusive Uhrzeit-Picker.
  3. Nach dem Speichern wird die Aufgabe auf dem Dashboard und im Kalender platziert.

#### US-3.2: Aufgabenstatus aktualisieren
- **User Story:** Als Student möchte ich den Status einer Aufgabe direkt in der Liste auf 'erledigt' setzen, damit ich meinen aktuellen Lernfortschritt sofort sehen kann.
- **Akzeptanzkriterien:**
  1. Jede Aufgabe in der Liste hat eine direkt anklickbare Checkbox.
  2. Klickt der Benutzer darauf, wechselt der Status sofort auf "Erledigt".
  3. Die Aufgabe wird visuell ausgegraut oder durchgestrichen dargestellt.

#### US-3.3: Unteraufgaben (Checklisten) nutzen
- **User Story:** Als Student möchte ich eine Hauptaufgabe in kleinere Unteraufgaben unterteilen, damit ich komplexe Projektarbeiten Schritt für Schritt abarbeiten kann.
- **Akzeptanzkriterien:**
  1. In der Detailansicht einer Aufgabe können beliebig viele Unteraufgaben hinzugefügt werden (nur Titel erforderlich).
  2. Unteraufgaben können unabhängig voneinander als "erledigt" markiert werden.
  3. Ein Fortschrittsbalken in der Hauptaufgabe zeigt das Verhältnis an (z. B. "2 von 5 erledigt").

---

### Epic 4: Deadlines & Ansichten

#### US-4.1: Deadline-Erinnerungen erhalten
- **User Story:** Als Student möchte ich vor dem Erreichen einer Deadline automatisch per Push-Benachrichtigung erinnert werden, damit ich keine Abgabefrist im Semesterstress verpasse.
- **Akzeptanzkriterien:**
  1. Beim Erstellen/Bearbeiten einer Aufgabe ist standardmäßig die Option "Erinnerung: 1 Tag vorher" aktiv.
  2. Der Benutzer kann zusätzliche Erinnerungen hinzufügen (z. B. "2 Stunden vorher").
  3. Die App triggert die Benachrichtigung exakt zur berechneten Zeit.

#### US-4.2: Chronologisches Dashboard nutzen
- **User Story:** Als Student möchte ich beim Öffnen der App alle unvollständigen Aufgaben nach Fälligkeit sortiert sehen, damit ich meine Prioritäten für den aktuellen Tag sofort erkenne.
- **Akzeptanzkriterien:**
  1. Der Startbildschirm listet alle unvollständigen Aufgaben auf.
  2. Die Sortierung erfolgt aufsteigend nach Datum (dringendste Aufgaben ganz oben).
  3. Überfällige Aufgaben werden farblich (z. B. rot) hervorgehoben.

#### US-4.3: Kalenderansicht nutzen
- **User Story:** Als Student möchte ich meine Aufgaben in einer monatlichen Kalenderansicht betrachten, damit ich meine Arbeitslast während der Prüfungsphase visuell besser einschätzen kann.
- **Akzeptanzkriterien:**
  1. Es gibt einen Navigationspunkt "Kalender".
  2. Aufgaben werden an ihren jeweiligen Fälligkeitstagen als farbige Blöcke (in der Kursfarbe) angezeigt.
  3. Ein Klick auf einen Kalendereintrag öffnet direkt die Detailansicht der Aufgabe.