# YappyUnc – Website (Support / Privacy / Impressum)

Statische Mini-Website für die von Apple verlangten URLs. Kein Build, kein JavaScript –
einfach drei HTML-Dateien. Wird kostenlos über **GitHub Pages** gehostet.

```
index.html       → Support  (Apple "Support URL")
privacy.html     → Privacy Policy  (Apple "Privacy Policy URL")
impressum.html   → Impressum (Pflicht in DE)
style.css        → gemeinsames Styling
```

## ⚠️ Vor dem Veröffentlichen ausfüllen
Diese Platzhalter in **allen** Dateien ersetzen (Suchen & Ersetzen):

- `CONTACT@EXAMPLE.COM` → deine echte Support-E-Mail
- In `impressum.html`: `DEIN VORNAME NACHNAME`, `STRASSE / POSTFACH`, `PLZ ORT`,
  und die `USt-IdNr.` (oder die Zeile entfernen, falls noch keine vorhanden)

> Hinweis: Der Repo ist **öffentlich**. Hier kommt **nur die Website** rein – niemals der
> Spiel-Quellcode.

## Veröffentlichen (einmalig, ~5 Min)

1. Auf github.com einen **neuen, öffentlichen Repo** anlegen, z. B. `yappyunc-site`.
2. In **diesem** Ordner (`yappyunc-site/`) im Terminal:

   ```sh
   git init
   git add .
   git commit -m "YappyUnc website: support, privacy, impressum"
   git branch -M main
   git remote add origin https://github.com/DEIN-USER/yappyunc-site.git
   git push -u origin main
   ```

3. Auf GitHub: **Settings → Pages → Source: „Deploy from a branch" → Branch: `main` / `(root)`** → Save.
4. Nach 1–2 Min ist die Seite live unter:
   `https://DEIN-USER.github.io/yappyunc-site/`

## Die URLs für App Store Connect
- **Support URL:** `https://DEIN-USER.github.io/yappyunc-site/`
- **Privacy Policy URL:** `https://DEIN-USER.github.io/yappyunc-site/privacy.html`

## Später: eigene Domain
Wenn du eine Studio-Domain hast (z. B. `studio.com`):
- In Settings → Pages → **Custom domain** eintragen (`studio.com` oder `yappyunc.studio.com`).
- Beim Domain-Anbieter einen `CNAME`-Eintrag auf `DEIN-USER.github.io` setzen.
- GitHub legt dann automatisch eine `CNAME`-Datei an und aktiviert HTTPS.
