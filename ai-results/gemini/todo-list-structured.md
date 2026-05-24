# Gemini Ergebnis: Simple To-do List - Structured Prompt

## Verwendeter Prompt

Erstelle Requirements und User Stories für eine einfache To-do-Listen-App.

Berücksichtige dabei:

- funktionale Requirements
- nicht-funktionale Requirements
- User Stories im Format: Als Benutzer möchte ich ..., damit ...
- eine klare und übersichtliche Struktur

## Ergebnis

# Software Requirements Specification (SRS) & User Stories
## Projekt: Simple To-Do-Listen-App

Dieses Dokument spezifiziert die funktionalen und nicht-funktionalen Anforderungen sowie die User Stories für die Entwicklung einer einfachen, intuitiven To-Do-Listen-App.

---

## 1. Funktionale Anforderungen (Functional Requirements)

Die funktionalen Anforderungen beschreiben die direkten Funktionen und Interaktionen, die das System dem Endbenutzer zur Verfügung stellen muss.

### 1.1 Aufgaben-Management (CRUD-Operationen)
* **FR-1 (Erstellen):** Das System muss es dem Benutzer ermöglichen, eine neue Aufgabe mit einem Titel (Pflichtfeld) zu erstellen.
* **FR-2 (Lesen/Anzeigen):** Das System muss alle aktiven und erledigten Aufgaben in einer übersichtlichen Liste anzeigen.
* **FR-3 (Aktualisieren):** Das System muss es dem Benutzer ermöglichen, den Titel einer bestehenden Aufgabe nachträglich zu bearbeiten.
* **FR-4 (Löschen):** Das System muss es dem Benutzer ermöglichen, eine Aufgabe unwiderruflich aus der Liste zu entfernen.

### 1.2 Status-Management
* **FR-5 (Als erledigt markieren):** Das System muss eine Option bieten, um eine Aufgabe als "erledigt" zu kennzeichnen.
* **FR-6 (Als offen markieren):** Das System muss es ermöglichen, eine bereits erledigte Aufgabe wieder in den Status "offen" zurückzusetzen.
* **FR-7 (Visuelle Trennung):** Erledigte Aufgaben müssen visuell (z. B. durch Streichung oder Ausgrauung) von offenen Aufgaben unterschieden werden.

### 1.3 Datenhaltung (Persistenz)
* **FR-8 (Lokale Speicherung):** Das System muss die Aufgaben lokal auf dem Gerät des Benutzers (z. B. via LocalStorage im Browser oder lokaler SQLite-Datenbank) speichern, damit die Daten nach dem Schließen der App oder einem Page-Reload erhalten bleiben.

---

## 2. Nicht-funktionale Anforderungen (Non-Functional Requirements)

Die nicht-funktionalen Anforderungen definieren die Qualitätsattribute, Rahmenbedingungen und technischen Eigenschaften des Systems.

### 2.1 Benutzbarkeit & Design (Usability)
* **NFR-1 (Intuitive Bedienung):** Die Benutzeroberfläche muss so minimalistisch und selbsterklärend sein, dass ein neuer Benutzer die App ohne Anleitung oder Einarbeitungszeit sofort bedienen kann.
* **NFR-2 (Barrierefreiheit):** Texte und interaktive Elemente müssen ausreichend Kontrast aufweisen (mindestens WCAG 2.1 AA Konformität für Textkontraste).
* **NFR-3 (Responsive Design):** Die Anwendung muss auf Smartphones (Mobile), Tablets und Desktop-Bildschirmen gleichermaßen vollständig und fehlerfrei dargestellt werden.

### 2.2 Leistung & Zuverlässigkeit (Performance & Reliability)
* **NFR-4 (Reaktionszeit):** Jede Benutzerinteraktion (z. B. das Hinzufügen oder Abhaken einer Aufgabe) muss innerhalb von maximal 100 Millisekunden visuell auf dem Bildschirm reflektiert werden (Echtzeit-Gefühl).
* **NFR-5 (Ladezeit):** Die App muss innerhalb von weniger als 1,5 Sekunden bei einer standardmäßigen 3G/4G-Verbindung vollständig geladen und einsatzbereit sein.

### 2.3 Technische Rahmenbedingungen & Wartbarkeit
* **NFR-6 (Plattform-Unabhängigkeit):** Da es sich um eine einfache App handelt, sollte sie plattformunabhängig als Web-App (SPA - Single Page Application) in allen modernen Browsern (Chrome, Safari, Firefox, Edge) laufen.
* **NFR-7 (Datenschutz):** Da die Speicherung rein lokal erfolgt, werden keine personenbezogenen Daten an externe Server übertragen (Offline-First-Ansatz).

---

## 3. User Stories

Die User Stories beschreiben die Anforderungen aus der Perspektive des Endbenutzers und folgen dem agilen Standard-Template. Jede User Story enthält klare Akzeptanzkriterien (Definition of Done).

### US-1: Aufgabe hinzufügen
* **Formulierung:** Als **Benutzer** möchte ich **eine neue Aufgabe schnell eingeben und speichern können**, damit **ich meine To-Dos nicht vergesse**.
* **Akzeptanzkriterien:**
    1. Es gibt ein klar ersichtliches Eingabefeld für den Aufgabentext.
    2. Die Aufgabe wird durch Drücken der Enter-Taste oder Klicken auf einen "Hinzufügen"-Button gespeichert.
    3. Ein leeres Eingabefeld kann nicht abgespeichert werden (Fehlerschutz).
    4. Nach dem Hinzufügen leert sich das Eingabefeld automatisch, damit sofort die nächste Aufgabe eingegeben werden kann.

### US-2: Aufgabenliste einsehen
* **Formulierung:** Als **Benutzer** möchte ich **eine Liste aller meiner Aufgaben sehen**, damit **ich den Überblick über meine offenen To-Dos behalte**.
* **Akzeptanzkriterien:**
    1. Alle hinzugefügten Aufgaben werden in einer vertikalen Liste untereinander dargestellt.
    2. Wenn noch keine Aufgaben existieren, wird ein motivationaler Platzhaltertext angezeigt (z. B. *"Du hast aktuell keine Aufgaben. Zeit zu entspannen!"*).

### US-3: Aufgabe als erledigt markieren
* **Formulierung:** Als **Benutzer** möchte ich **Aufgaben als erledigt abhhaken können**, damit **ich meinen Fortschritt sehe und weiß, was bereits geschafft ist**.
* **Akzeptanzkriterien:**
    1. Jede Aufgabe besitzt eine Checkbox oder ein vergleichbares interaktives Element zum Abhaken.
    2. Klickt man darauf, ändert sich der Status auf "erledigt".
    3. Der Text der erledigten Aufgabe wird visuell durchgestrichen und die Deckkraft leicht reduziert.

### US-4: Aufgabe löschen
* **Formulierung:** Als **Benutzer** möchte ich **eine Aufgabe dauerhaft entfernen können**, damit **ich Fehler korrigieren oder irrelevante Einträge aus meiner Liste entfernen kann**.
* **Akzeptanzkriterien:**
    1. Neben jeder Aufgabe befindet sich ein Lösch-Symbol (z. B. ein Mülleimer-Icon).
    2. Das Lösch-Symbol wird beim Hovern (Desktop) oder dauerhaft (Mobil) angezeigt.
    3. Nach dem Klicken auf das Symbol verschwindet die Aufgabe sofort und dauerhaft aus der Liste.

### US-5: Persistenz nach dem Neuladen
* **Formulierung:** Als **Benutzer** möchte ich, **dass meine Aufgaben beim Schließen des Browsers gespeichert bleiben**, damit **ich meine Liste nicht jedes Mal neu eintippen muss**.
* **Akzeptanzkriterien:**
    1. Beim Schließen des Tabs oder Aktualisieren der Seite (F5) bleiben alle Aufgaben (inklusive ihres Status) erhalten.
    2. Die Daten werden ohne serverseitiges Login direkt im Browser-Speicher abgelegt.

---

## 4. Priorisierungsmatrix (Optionaler Anhang)

Für eine inkrementelle Entwicklung (MVP - Minimum Viable Product) wird folgende Priorisierung der User Stories empfohlen:

| ID | Feature / User Story | Priorität | Release-Phase |
| :--- | :--- | :--- | :--- |
| **US-1** | Aufgabe hinzufügen | **Must-have** | MVP (Phase 1) |
| **US-2** | Aufgabenliste einsehen | **Must-have** | MVP (Phase 1) |
| **US-3** | Aufgabe als erledigt markieren | **Must-have** | MVP (Phase 1) |
| **US-4** | Aufgabe löschen | **Should-have** | MVP (Phase 1) |
| **US-5** | Persistenz (Local Storage) | **Must-have** | MVP (Phase 1) |
| **FR-3** | Aufgabe bearbeiten (Titel ändern) | **Could-have** | Post-MVP (Phase 2) |