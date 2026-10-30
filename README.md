# Winter-Arcade – Premium Landingpage (DE/EN)

Statische, GitHub-Pages-fertige Website für die **Winter-Arcade** (Flondy). Keine npm-Installation, kein Build-Schritt, kein Server-Backend. Enthält `index.html`, `datenschutz.html`, `app-datenschutz.html`, `impressum.html`, `css/style.css`, `js/main.js` und lokal optimierte Bilder im Ordner `assets/`.

## Lokal testen

`index.html` direkt im Browser öffnen. Für alle Funktionen (insbesondere Link-/URL-Verhalten) empfiehlt sich im Ordner ein lokaler Webserver, z. B. `python -m http.server 8000` und anschließend `http://localhost:8000/` öffnen.

## GitHub Pages hochladen

1. Repository erstellen (z. B. `winter-arcade`), alle Dateien und Ordner **aus diesem ZIP** in das Repo-Root hochladen.
2. GitHub: Settings → Pages → Build and deployment → Deploy from a branch → `main` / `(root)` → Save.
3. Veröffentlichte URL öffnen und alle internen Links sowie Smartphone-Ansichten prüfen. Für Projekt-Repositories heißt die Adresse normalerweise `https://<account>.github.io/<repository>/`. Die Seite verwendet **relative Pfade** und funktioniert deshalb auch unter einem Unterverzeichnis.
4. Vor der öffentlichen Veröffentlichung bitte die unten genannten rechtlichen und technischen Punkte erledigen.

## ZWINGEND vor Veröffentlichung

- `impressum.html`: `[VOR- UND NACHNAME / RECHTLICHE FIRMENBEZEICHNUNG]`, gültige ladungsfähige Geschäftsanschrift, geschäftliche E-Mail und ggf. Register-/Steuerangaben ausfüllen (DE + EN).
- `datenschutz.html`: Verantwortlichen/Kontaktangaben ergänzen (DE + EN); prüfen, ob die Website tatsächlich auf GitHub Pages läuft. Bei anderem Hosting die Datenschutzdetails ändern.
- Die Angaben sind **Muster/Entwürfe**, keine verbindliche Rechtsberatung. Vor öffentlichem Einsatz für konkrete Firma, Hosting und SDKs überprüfen lassen.
- Die separate `app-datenschutz.html` ist ein ausdrücklich gekennzeichneter **Entwurf für die künftige App**. Vor Store-Einreichung müssen tatsächliche SDKs, Berechtigungen und Datenflüsse überprüft und sämtliche Platzhalter vervollständigt werden. Die Website-Datenschutzerklärung `datenschutz.html` beschreibt nur die Website.
- Store-Links sind ausdrücklich noch nicht freigeschaltet, da gemäß Projektdokumentation kein Release bestätigt ist. Erst nach Veröffentlichung die beiden deaktivierten Store-Pills in `index.html` in echte, verifizierte Links umwandeln.
- Die aktuellen Marketing-Screenshots sind KI-generierte **Konzeptillustrationen**, keine echten Gameplay-Screenshots. Später durch echte Screenshots aus dem fertig getesteten Spiel ersetzen.
- Abgleich mit aktuellem Unity-Build: Die Dokumentation vom 30.10.2026 bestätigt einen Test der C#-Implementierung gegen Stubs, aber keine echten Unity-Editor-/Smartphone-Tests.

## Datenschutzfreundliche technische Umsetzung

- Statische HTML/CSS/JS-Seite ohne Analytics, Tracking, externe Fonts, Cookie-Banner, Social-Embeds oder Kontaktformular.
- Alle Bilder werden lokal gehostet. Ausgehende externe Links werden erst auf Nutzeraktion geöffnet.
- Sprachumschaltung mittels URL-Parameter `?lang=en`, ohne LocalStorage/Cookies. Interne Rechtstexte übernehmen die Sprache.
- GitHub Pages protokolliert laut GitHub bei einem Besuch die IP-Adresse zu Sicherheitszwecken (https://docs.github.com/en/pages/getting-started-with-github-pages/what-is-github-pages).

## Bildmaterial

Die verwendeten KI-generierten Originalillustrationen wurden im Rahmen dieser Unterhaltung erstellt und in WebP für eine schlanke Website umgewandelt. Das App-Symbol und alle fünf Spielgrafiken sind im `assets/`-Ordner enthalten. Die Seite nutzt keine extern geladenen Bild- oder Schriftdateien.

## Vorbereitete Funktionen

- Desktop-/Tablet-/Smartphone-Layout, Touch-freundliches Menü
- Deutsch/Englisch umschaltbar, rechtliche Seiten in beiden Sprachen
- Fünf Spiele-Karten mit aus der Projektdokumentation abgeleiteten Beschreibungen
- Konzeptbild-Slider mit Großbildansicht (Dialog)
- FAQ, Roadmap/Projektstatus, Studiosammlung-Link
- Accessibility: semantische Überschriften, Skip-Link, Tastaturbedienbarkeit, Reduced Motion, Bild-Alternativtexte

## Welche Spielinhalte tatsächlich dokumentiert sind

Quelle: `Winter-Arcade_Projektdokumentation.pdf` vom 30. Oktober 2026. Die fünf Minispiele: Rolling Snowball, Pinguin-Rutschpartie, Frostbound Survivors, Pinguin-Schubsen, Echo Run. Es gibt einen mobilen Browserprototyp und nach C# übertragenes Unity-Projekt mit selbst gezeichneten Formen. Store-Builds und finaler Premium-Look sind noch nicht dokumentiert.
