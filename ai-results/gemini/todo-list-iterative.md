# Gemini Ergebnis: Simple To-do List - Iterative Prompt

## Verwendete Prompts

### Prompt 1

Erstelle Requirements und User Stories für eine einfache To-do-Listen-App.

### Prompt 2

Überarbeite das Ergebnis und ergänze fehlende funktionale und nicht-funktionale Requirements.

### Prompt 3

Verbessere die User Stories und achte darauf, dass sie im Format „Als Benutzer möchte ich ..., damit ...“ geschrieben sind.

## Ergebnis

# Requirements und User Stories für eine einfache To-do-Listen-App (v2.1)

Dieses Dokument enthält die funktionalen und nicht-funktionalen Anforderungen sowie die User Stories für die Entwicklung einer einfachen, intuitiven To-do-Listen-App. Das Ziel des Produkts ist es, Nutzern eine unkomplizierte, verlässliche Möglichkeit zu bieten, tägliche Aufgaben zu strukturieren und zu verwalten.

---

## 1. Produkt-Übersicht & Zielsetzung
Die To-do-Listen-App ist eine leichtgewichtige Anwendung (Web/Mobile), die es Anwendern ermöglicht, Aufgaben (Todos) schnell zu erfassen, zu organisieren und als erledigt zu markieren. Der Fokus liegt auf maximaler Benutzerfreundlichkeit, minimaler Ladezeit, Robustheit gegen Fehlbedienung und einer klaren, ablenkungsfreien Benutzeroberfläche.

---

## 2. Funktionale Anforderungen (Functional Requirements)

### 2.1 Aufgabenverwaltung & CRUD-Operationen (Core MVP)
* **FR-1 (Erstellen):** Das System muss es dem Nutzer erlauben, eine neue Aufgabe mit einem Titel zu erstellen.
* **FR-2 (Eingabe-Validierung):** Das System darf keine leeren Aufgaben oder reinen Whitespaces (Leerzeichen) als Titel akzeptieren. Der Titel muss auf maximal 150 Zeichen begrenzt sein, um UI-Brüche zu verhindern.
* **FR-3 (Anzeigen):** Das System muss eine Liste aller aktiven (unerledigten) Aufgaben standardmäßig anzeigen.
* **FR-4 (Zustandsänderung):** Das System muss es dem Nutzer ermöglichen, eine Aufgabe als "erledigt" zu markieren und diesen Schritt bei Bedarf wieder rückgängig zu machen.
* **FR-5 (Visuelles Feedback):** Erledigte Aufgaben müssen visuell sofort als solche gekennzeichnet werden (z. B. durchgestrichen, verringerte Opazität).
* **FR-6 (Aktualisieren/Editieren):** Der Nutzer muss in der Lage sein, den Titel einer bestehenden Aufgabe nachträglich per Doppelklick oder "Bearbeiten"-Button zu ändern.
* **FR-7 (Löschen):** Das System muss es dem Nutzer erlauben, eine Aufgabe unwiderruflich aus der Liste zu löschen.
* **FR-8 (Massen-Aktionen):** Das System sollte eine Funktion bereitstellen, mit der alle als "erledigt" markierten Aufgaben mit einem einzigen Klick gelöscht werden können ("Erledigte aufräumen").

### 2.2 Filtern & Sortieren (MVP+)
* **FR-9 (Filterung):** Der Nutzer muss die Liste nach Status filtern können: "Alle", "Aktiv" (offen) und "Erledigt".
* **FR-10 (Sortierung):** Neu erstellte Aufgaben müssen standardmäßig chronologisch ganz oben in der Liste der aktiven Aufgaben angeheftet werden.

### 2.3 Datenhaltung & Ausfallsicherheit (Data & State)
* **FR-11 (Lokale Speicherung):** Die Aufgaben müssen lokal auf dem Gerät des Nutzers persistent gespeichert werden (z. B. via `localStorage` oder `IndexedDB` im Browser).
* **FR-12 (Zustandswiederherstellung):** Beim plötzlichen Schließen des Browsers, einem Tab-Wechsel oder App-Crash darf kein Datenverlust auftreten; der letzte Zustand muss beim nächsten Start vollständig wiederhergestellt werden.

---

## 3. Nicht-funktionale Anforderungen (Non-Functional Requirements)

### 3.1 Usability & User Experience (UX)
* **NFR-1 (Effizienz):** Die Benutzeroberfläche muss intuitiv und ohne Anleitung bedienbar sein. Das Erstellen einer Aufgabe darf maximal 1 Klick (oder `Enter`-Tastendruck) nach der Texteingabe erfordern.
* **NFR-2 (Fehlertoleranz):** Das versehentliche Löschen einer Aufgabe muss durch ein kurzzeitiges Pop-up ("Rückgängig machen" / Toast-Notification) für mindestens 5 Sekunden reversibel sein.
* **NFR-3 (Leerzustände / Empty States):** Wenn keine Aufgaben in der gewählten Filteransicht vorhanden sind, muss ein klarer, motivationaler Platzhaltertext angezeigt werden (z. B. *"Keine offenen Aufgaben. Zeit zum Entspannen!"*).

### 3.2 Performance & Skalierbarkeit
* **NFR-4 (Ladezeit):** Die App muss (bei lokaler Ausführung/Caching) innerhalb von weniger als 500ms initial einsatzbereit sein.
* **NFR-5 (Reaktionszeit):** UI-Interaktionen (z. B. das Abhaken oder Löschen einer Aufgabe) müssen visuell verzögerungsfrei innerhalb von maximal 50ms gerendert werden.
* **NFR-6 (Skalierbarkeit der Liste):** Die App muss flüssig und ohne Performance-Einbußen (Lagging beim Scrollen oder Tippen) mit bis zu 1.000 lokal gespeicherten Aufgaben umgehen können.

### 3.3 Kompatibilität & Design (Responsiveness)
* **NFR-7 (Responsive Design):** Die App muss auf Smartphones (ab 320px Breite), Tablets und Desktop-Monitoren voll funktionsfähig und fehlerfrei dargestellt werden (Mobile-First-Ansatz).
* **NFR-8 (Cross-Browser-Kompatibilität):** Die Anwendung muss auf allen modernen Browsern (Chrome, Safari, Firefox, Edge) in den jeweils letzten 3 Major-Versionen identisch funktionieren.

### 3.4 Barrierefreiheit (Accessibility) & Sicherheit
* **NFR-9 (A11y - Kontrast & Bedienung):** Alle UI-Elemente müssen den WCAG 2.1 AA-Richtlinien entsprechen (z. B. Kontrastverhältnis von mindestens 4.5:1 für Text). Die App muss vollständig ohne Maus, rein über die Tastatur (`Tab`, `Enter`, `Space`, `Esc`), bedienbar sein.
* **NFR-10 (Screenreader):** Interaktive Elemente (Checkboxes, Löschen-Buttons) müssen über korrekte HTML-Attribute (`aria-label`, `aria-checked`) verfügen, damit sie von Screenreadern fehlerfrei interpretiert werden können.
* **NFR-11 (Datenschutz & Sicherheit):** Da es sich um eine rein clientseitige App handelt, werden ohne explizite Zustimmung des Nutzers keine personenbezogenen Daten an externe Server übermittelt (DSGVO-konform per Design). Eingaben müssen gegen XSS (Cross-Site Scripting) geschützt werden (Sanitizing des Inputs).

---

## 4. User Stories

### Epic: Kern-Aufgabenverwaltung

#### US-1: Aufgabe valide erstellen
* **Als** strukturierter Benutzer 
* **möchte ich** eine neue Aufgabe mit einem kurzen, validen Text anlegen können, 
* **damit** ich mich später verlässlich an diese Erledigung erinnere.

**Akzeptanzkriterien:**
1. Ein prominentes Text-Eingabefeld mit dem Platzhalter *"Neue Aufgabe hinzufügen..."* ist beim App-Start sofort fokussiert.
2. Ein Klick auf ein "+"-Symbol oder das Drücken der `Enter`-Taste erstellt die Aufgabe.
3. Nach der Erstellung wird das Eingabefeld automatisch geleert.
4. Drückt der Nutzer `Enter` bei leerem Feld oder reinen Leerzeichen, passiert nichts (keine Erstellung einer "leeren" Aufgabe).
5. Eingaben, die länger als 150 Zeichen sind, werden im Eingabefeld blockiert oder abgeschnitten (mit visuellem Zeichenzähler).

---

#### US-2: Aufgabenliste filtern
* **Als** vielbeschäftigter Benutzer 
* **möchte ich** meine To-do-Liste nach dem Status „Alle“, „Aktiv“ und „Erledigt“ filtern können, 
* **damit** ich jederzeit gezielt nur die für mich im Moment relevanten Aufgaben sehe.

**Akzeptanzkriterien:**
1. Es gibt eine Filterleiste mit drei Optionen: "Alle", "Aktiv", "Erledigt".
2. Der aktive Filter wird visuell hervorgehoben (z. B. durch Fettdruck oder Hintergrundfarbe).
3. Wechselt man auf "Aktiv", werden *nur* die unerledigten Aufgaben angezeigt.
4. Ist eine Liste leer (z. B. keine erledigten Aufgaben vorhanden), wird ein entsprechender "Empty State"-Text eingeblendet.

---

#### US-3: Aufgabe bearbeiten (Inline Edit)
* **Als** fehlerbehafteter Benutzer 
* **möchte ich** den Text einer bereits existierenden Aufgabe nachträglich ändern können, 
* **damit** ich Tippfehler oder Planänderungen korrigieren kann, ohne die Aufgabe komplett neu erstellen zu müssen.

**Akzeptanzkriterien:**
1. Ein Doppelklick auf den Text einer Aufgabe verwandelt den Text in ein editierbares Eingabefeld.
2. Während des Editierens werden die Checkbox und das Löschen-Symbol temporär ausgeblendet.
3. Drücken von `Enter` oder das Verlassen des Feldes (`Blur`-Event) speichert den geänderten Text, sofern dieser valide ist.
4. Drücken von `Esc` bricht den Editier-Vorgang ab und stellt den alten Text wieder her.

---

#### US-4: Aufgabe als erledigt markieren & reaktivieren
* **Als** ergebnisorientierter Benutzer 
* **möchte ich** Aufgaben flexibel abhaken und den Haken bei Bedarf auch wieder entfernen können, 
* **damit** der aktuelle Status meiner Aufgaben immer exakt meinem realen Arbeitsfortschritt entspricht.

**Akzeptanzkriterien:**
1. Vor jedem Aufgabentext befindet sich eine Checkbox.
2. Klickt der Benutzer darauf, wird die Aufgabe abgehakt, der Text durchgestrichen und die Aufgabe visuell abgeschwächt.
3. Befindet sich der Benutzer im Filter "Aktiv", verschwindet die soeben abgehakte Aufgabe nach einer kurzen Animation (ca. 300ms) aus der Ansicht.
4. Ein erneuter Klick auf die Checkbox einer erledigten Aufgabe setzt ihren Status zurück auf "Aktiv".

---

#### US-5: Aufgabe löschen mit Absicherung
* **Als** ordnungsliebender Benutzer 
* **möchte ich** eine Aufgabe unwiderruflich aus meiner Liste entfernen sowie eine versehentliche Löschung direkt rückgängig machen können, 
* **damit** meine Liste stets aufgeräumt bleibt und ich keine Daten durch Fehlklicks verliere.

**Akzeptanzkriterien:**
1. Am rechten Rand jeder Aufgabe befindet sich ein "Löschen"-Symbol (Mülleimer-Icon), das für Screenreader als "Aufgabe löschen" benannt ist.
2. Nach dem Klick verschwindet die Aufgabe sofort aus der Liste.
3. Es erscheint eine Toast-Nachricht am unteren Bildschirmrand: *"Aufgabe gelöscht. [Rückgängig]"*.
4. Klickt der Benutzer innerhalb von 5 Sekunden auf "Rückgängig", wird die Aufgabe an exakt derselben Stelle der Liste mit all ihren Daten wiederhergestellt.

---

#### US-6: Tastatur-Steuerung (Barrierefreiheit)
* **Als** motorisch eingeschränkter Benutzer 
* **möchte ich** die gesamte Anwendung ohne Maus nur mit der Tastatur bedienen können, 
* **damit** ich die App barrierefrei und ohne Einschränkungen nutzen kann.

**Akzeptanzkriterien:**
1. Mit der `Tab`-Taste kann sequenziell durch das Eingabefeld, die Filter-Buttons, die Checkboxen und die Lösch-Buttons navigiert werden.
2. Das aktuell fokussierte Element muss einen deutlich sichtbaren Fokus-Rahmen (Focus Outline) aufweisen.
3. Ist eine Checkbox fokussiert, kann sie mit der `Leertaste` (Space) umgeschaltet werden.
4. Ist ein Lösch-Button fokussiert, löst die `Enter`-Taste den Löschvorgang aus.

---

## 5. Zukünftiges Backlog (v3.0+)
* **Kategorien/Projekte:** Erstellen mehrerer getrennter To-do-Listen (z. B. "Privat", "Arbeit").
* **Fälligkeit & Erinnerung:** Hinzufügen von Deadlines und Push-Benachrichtigungen im Browser.
* **Cloud-Synchronisation:** Optionaler Login, um Listen verschlüsselt über mehrere Endgeräte hinweg synchron zu halten.