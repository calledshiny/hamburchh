# ⚓ Hamburch

**Amtliches Reisedossier** — Gruppenreise Hamburg 2025

Ein digitales Reisedossier im Stil der Hamburger Hafenbehörde. Alle wichtigen Entscheidungen der Reisegruppe an einem Ort.

---

## Module

| Formular | Beschreibung |
|----------|-------------|
| `index.html` | Startseite & Übersicht |
| `fahrt.html` | Fahrzeugeinteilung — wer fährt mit wem (Voting) |
| `programm.html` | Aktivitäten vorschlagen & abstimmen |
| `kasse.html` | Gemeinschaftskasse & automatischer Ausgleich |

---

## Setup

### 1. Firebase konfigurieren
In `firebase.js` die eigene Firebase-Config eintragen:
```js
export const firebaseConfig = {
  apiKey: "...",
  databaseURL: "...",
  // ...
};
```

Firebase Realtime Database Regeln auf offen setzen (für privaten Gebrauch):
```json
{
  "rules": {
    ".read": true,
    ".write": true
  }
}
```

### 2. Hosting
Einfachste Option: **Netlify Drop**
- netlify.com/drop aufrufen
- Den `hamburch/` Ordner reinziehen
- Fertiger Link

---

## Design System

Alle Seiten verwenden `style.css` mit dem gemeinsamen Design System:
- **Bebas Neue** — Überschriften, Labels, Zahlen
- **Special Elite** — Fließtext, amtlicher Charakter
- Farbpalette: Papiergelb, Tinte, Navy, Gold, Rost

---

*Ausgestellt im Auftrag der Reisegruppe · Hamburg 2025*
