# <p align="center">Wirtschaftsquiz - IDPA Projekt 🎓</p>

<p align="center">
  <img src="https://files.catbox.moe/czgpy5.gif" alt="wirtschaftsquiz gif"/>
</p>

<p align="center"><strong>Wirtschaftsquiz</strong> ist eine interaktive Plattform auf Deutsch zum Erstellen und Durchführen von Quizzen mit einer UI/UX-orientierten Interface, entwickelt im Rahmen einer Interdisziplinären Projektarbeit (IDPA). Das Projekt konzentriert sich auf die Wissensüberprüfung im Bereich Wirtschaft, kann aber dank seiner flexiblen Struktur für thematische Tests jeglicher Art verwendet werden.</p>

---

## 🛠️ Technologie-Stack

- **Frontend:**
  - HTML5, CSS3
  - Vanilla JavaScript
- **Backend:**
  - Node.js
  - Express.js (REST API)
- **Datenbank:**
  - Lokaler JSON-basierter Speicher

---

## 🚀 Installation & Start

Befolgen Sie diese Schritte, um das Projekt auf Ihrem lokalen Rechner bereitzustellen.

### Voraussetzungen

- Installiertes [Node.js](https://nodejs.org/) (Version 14 oder höher).

### Installationsschritte

1. **Repository klonen:**

   ```bash
   git clone https://github.com/y4lexzs/wirtschaftsquiz.git
   cd wirtschaftsquiz
   ```

2. **Abhängigkeiten installieren:**

   ```bash
   npm install
   ```

3. **Umgebung einrichten:**
   Öffnen Sie `assets/js/storage.js` und stellen Sie sicher, dass `API_URL` auf Ihren Server zeigt (Standard für lokale Entwicklung ist `http://localhost:3000/api`).

   ```javascript
   // assets/js/storage.js
   const API_URL = "http://localhost:3000/api";
   ```

4. **Server starten:**

   ```bash
   npm start
   ```

   Der Server startet auf Port `3000`.

5. **Anwendung öffnen:**
   Navigieren Sie in Ihrem Browser zu `http://localhost:3000`.

---

## 📖 Benutzerhandbuch

1. **Erste Schritte:**

   - Öffnen Sie die Anwendung und registrieren Sie sich über das Formular `auth.html`.
   - Nach der Anmeldung gelangen Sie auf `index.html` oder `dashboard.html`.

2. **Inhaltserstellung:**

   - Gehen Sie zur **Fragensammlung** (`question-bank.html`) und erstellen Sie einige Themen und Fragen.
   - Verwenden Sie den **Quiz-Editor** (`quiz-editor.html`), um Fragen zu einem vollständigen Quiz zusammenzustellen.

3. **Tests durchführen:**

   - Teilen Sie den Quiz-Code oder Link mit den Teilnehmern.
   - Teilnehmer absolvieren den Test auf der Seite `take-quiz.html`.
   - Die Ergebnisse sind sofort nach Abschluss auf der Seite `review.html` verfügbar.

---

## ✨ Hauptfunktionen

### 🔐 Benutzer & Authentifizierung

- **Registrierung & Anmeldung:** Einfaches System zur Benutzerregistrierung und -autorisierung.
- **Personalisierung:** Jeder Benutzer (Lehrer oder Schüler) hat sein eigenes Profil.
- **Sicherheit:** Benutzerdaten werden in einer integrierten JSON-Datenbank gespeichert.

### 📚 Inhalt

- **Themen:** Erstellen und Verwalten verschiedener Themen.
- **Fragensammlung:** Hinzufügen, Bearbeiten und Löschen von Fragen.
- **Fragetypen:** Möglichkeit zur Erstellung verschiedener Fragetypen (Wahr/Falsch, Multiple Choice, Texteingabe).
- **Quizze:** Erstellen und Verwalten von Quizzen.

### 📝 Quiz-Editor

- **Baukasten:** Intuitive Oberfläche zum Zusammenstellen von Quizzen aus erstellten Fragen.
- **Flexibilität:** Möglichkeit, spezifische Fragen aus der Sammlung für den Test auszuwählen.
- **Teilen:** Einzigartige Codes für schnelles Teilen und Zugriff auf Quizze.

### 🚀 Quiz-Teilnahme & Analysen

- **Interaktiver Player:** Bequeme Oberfläche zum Durchführen von Tests.
- **Sofortiges Feedback:** Benutzer sehen die Ergebnisse sofort.
- **Überprüfung:** Detaillierte Ansicht der richtigen und falschen Antworten nach Abschluss.

---

## 📂 Projektstruktur

```
IDPA_readme/
├── assets/                 # Statische Ressourcen
│   ├── css/styles.css      # Stile
│   └── js/                 # App-Logik (API, UI-Controller)
│       ├── storage.js      # API & Datenbank-Interaktion
│       └── ...             # Skripte für jede Seite und mehr
├── data/                   # Datenspeicher (automatisch erstellt)
│   └── db.json             # Hauptdatenbank (JSON)
├── node_modules/           # Projektabhängigkeiten
├── auth.html               # Anmelde-/Registrierungsseite
├── dashboard.html          # Dashboard
├── index.html              # Startseite
├── new-question.html       # Seite zur Fragenerstellung
├── question-bank.html      # Fragensammlung
├── quiz-editor.html        # Quiz-Editor
├── review.html             # Seite zur Ergebnisüberprüfung
├── server.js               # Backend-Server-Einstiegspunkt
├── take-quiz.html          # Quiz-Player-Seite
├── package.json            # Projektmanifest & Skripte
├── LICENSE                 # Lizenzdatei
└── README.md               # Projektdokumentation
```

---

## 🤝 Mitwirkung

Wenn Sie das Projekt verbessern möchten, bitte:

1. Forken Sie das Repository.
2. Erstellen Sie einen Branch für Ihr Feature (`git checkout -b feature/TollesFeature`).
3. Committen Sie Ihre Änderungen (`git commit -m 'Füge ein TollesFeature hinzu'`).
4. Pushen Sie den Branch (`git push origin feature/TollesFeature`).
5. Öffnen Sie einen Pull Request.

---

## 📄 Lizenz

Dieses Projekt wird unter der MIT-Lizenz vertrieben. Siehe die Datei [LICENSE](LICENSE) für Details.

---

<p align="center">*Entwickelt mit ❤️ im Rahmen des IDPA-Bildungsprojekts.*</p>
