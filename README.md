# Cold Call Starterkit – Landing Page (GitHub Pages)

Kostenlose Lead-Magnet-Seite im Korwin Corporate Design, gebaut für LinkedIn-Traffic.
Statische Seite, keine Server nötig.

---

## 1. Repository anlegen

1. Auf [github.com](https://github.com) einloggen → **New repository**
2. Name: `starterkit` (ergibt später die URL `.../starterkit/`)
3. Sichtbarkeit: **Public** (Pflicht für kostenlose GitHub Pages)
4. **Create repository**

## 2. Dateien hochladen

Im neuen Repo auf **Add file → Upload files** und diese Struktur hochladen:

```
index.html
Cold-Call-Starterkit_Korwin.pdf
assets/christian-korwin.jpg
assets/linkedin-preview.png
```

Dann unten auf **Commit changes**.

## 3. GitHub Pages aktivieren

1. Im Repo: **Settings → Pages**
2. Unter *Build and deployment → Source*: **Deploy from a branch**
3. Branch: **main**, Ordner: **/ (root)** → **Save**
4. Nach 1–2 Minuten erscheint oben die Live-URL:
   `https://DEIN-BENUTZERNAME.github.io/starterkit/`

## 4. Drei Stellen in `index.html` anpassen

| Stelle | Was eintragen |
|---|---|
| `og:image` und `og:url` (Zeile ~18–20) | Deine echte GitHub-Pages-URL – sonst zeigt LinkedIn keine Vorschau |
| `FORM_ENDPOINT` (im `<script>` ganz unten) | Deine Formular-URL, siehe Schritt 5 |
| `impressum.html` / `datenschutz.html` im Footer | Diese beiden Seiten musst du noch anlegen (Pflicht, siehe unten) |

Bearbeiten geht direkt auf GitHub: Datei anklicken → Stift-Symbol → ändern → **Commit changes**.

## 5. E-Mail-Adressen empfangen

GitHub Pages ist rein statisch – es kann keine Daten speichern. Nutze einen kostenlosen Formular-Dienst:

**Empfehlung: [Formspree](https://formspree.io)** (kostenlos bis 50 Einsendungen/Monat)
1. Registrieren → **New Form** → Name z. B. „Starterkit"
2. Du bekommst eine URL wie `https://formspree.io/f/xayzqwer`
3. Diese in `index.html` bei `FORM_ENDPOINT` eintragen
4. Fertig – jede Anmeldung landet in deinem Postfach

**Alternative für echtes E-Mail-Marketing:** [MailerLite](https://mailerlite.com) oder [Brevo](https://brevo.com) – dort bekommst du zusätzlich automatische Willkommens-Mails und eine echte Verteilerliste. Beide bieten ebenfalls eine Formular-URL, die du an derselben Stelle einträgst.

> Der Download funktioniert bewusst auch dann, wenn der Formular-Dienst gerade nicht erreichbar ist – niemand soll ohne sein PDF dastehen.

## 6. Impressum & Datenschutz (Pflicht)

Lege im Repo zwei weitere Dateien an: `impressum.html` und `datenschutz.html`.
Am einfachsten: `index.html` kopieren, Inhalt ersetzen, Struktur behalten.
Sobald du E-Mail-Adressen sammelst und die Seite bewirbst, sind beide rechtlich erforderlich (DSGVO).

## 7. Eigene Domain (optional)

Statt `github.io` geht auch `starterkit.korwin-advisory.ch`:
1. **Settings → Pages → Custom domain**: `starterkit.korwin-advisory.ch` eintragen
2. Beim Domain-Anbieter einen **CNAME-Eintrag** setzen:
   `starterkit` → `DEIN-BENUTZERNAME.github.io`
3. **Enforce HTTPS** aktivieren (erscheint nach einigen Minuten)

## 8. Auf LinkedIn teilen

1. Link im LinkedIn-Beitrag posten – die Vorschaugrafik erscheint automatisch
2. Falls noch die alte Vorschau angezeigt wird: [LinkedIn Post Inspector](https://www.linkedin.com/post-inspector/) öffnen, URL eingeben, **Inspect** → Cache wird erneuert
3. Den Link zusätzlich in dein LinkedIn-Profil setzen: **Profil bearbeiten → Website hinzufügen**

---

## Anderen Lead-Magnet ausliefern

PDF austauschen und drei Stellen anpassen:
1. Neue PDF-Datei ins Repo hochladen
2. In `index.html` beim Download-Button `href="…pdf"` auf den neuen Dateinamen ändern
3. Titel, Hero-Texte und die vier Häkchen-Punkte anpassen

## Design-Regeln (Korwin CD)

- Farben: Espresso `#211D18`, Bernstein `#B8793A`, Bernstein tief `#A66C31`, Off-White `#F7F5F0`, Creme `#F1EEE7`, Body-Grau `#5E6570`, Haarlinie `#E6E1D6`
- Schriften: **Anton** für Headlines, **Inter** für alle Texte, **Fraunces Italic** ausschließlich für Zitate
- Gender-Linie: Du-Form bevorzugen, neutrale Begriffe („Menschen im Vertrieb"), eine ausgeschriebene Doppelnennung pro Seite, keine Genderzeichen im Wortinneren
