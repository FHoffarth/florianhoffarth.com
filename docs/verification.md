# V1 — technische Prüfung

Prüfdatum: 2026-09-05. Basis: `main` bei
`ec331a3751670cd8d9a84c4a9c00e390500cc070`, Repository `FHoffarth/florianhoffarth.com`.
Der Ausgangsstand enthielt ausschließlich README.md; keine vorhandene Website,
keine Tests, keine Repository-Anweisungen und keine CI-/Deployment-Workflows.

## Architektur und Übernahme

Die ZIP enthielt neben der Claude-Offline-Hülle bereits ein statisches `site/`-Paket.
Dieses wurde als Ausgangsbasis genutzt. Nicht übernommen: support.js, x-dc-/helmet-
Hülle, Design-System-Bundle, Upload-PDF, Thumbnail und Sync-Notizen.
Alle öffentlichen Dateien liegen im Repository-Root bzw. assets/.

Der Text der Startseite stimmt nach Normalisierung von Leerraum mit `site/index.html`
aus der ZIP überein, abgesehen von der beabsichtigten Überschrift
„Forschung & Publikationen“. Das Porträt ist byteidentisch.
Alle drei Berufspositionen, sechs Aufgaben der aktuellen Position, drei Projekte
mit ihren vorgegebenen Statusangaben, Publikation, Abschlüsse, Sprachen und echten
Profilverweise sind erhalten. Keine neuen biografischen Fakten ergänzt.

Off-White, Slate, Blau, Systemfont-Stack, großzügiger Weißraum, zweispaltige
Desktop-Gliederung, feine Linien und Porträt-Zuschnitt folgen dem Entwurf.
Die fünfstufige Leitidee bleibt mit 13 px und gedeckter Farbe sekundär zum Hero.

Gezielte technische Anpassungen:

- Skip-Link führt auf das fokussierbare main-Element, Fokus sichtbar.
- Mobile Porträtgröße 112 × 140 statt 152 × 190 px.
- Mobile `.wrap`-Regel ändert nur horizontale Abstände: Footer-Padding bleibt erhalten.
- Main-Padding mit passender Spezifität wiederhergestellt; im Export überschrieben.
- 112-px-Abstände zwischen nachfolgenden Desktop-Abschnitten und 22-px-Abstand
  oberhalb der Leitidee entsprechen wieder dem Offline-Design.
- Footer-Linie auf den Seitenfooter begrenzt, keine zusätzliche Linie im Literaturzitat.
- Mobile Legal-Überschrift nach Desktop-Regel platziert, damit 26 px wirksam bleiben.
- Überflüssige Sprach- und TODO-Stile entfernt. Die deutsche Navigation war im
  mitgelieferten site/-Paket bereits vorhanden und wurde bewahrt.
- Legal-Seiten im selben Stil neu gefasst: private Daten aus TODOs, pauschale
  Haftungsaussagen und unbelegte Hosting-/E-Mail-Aussagen entfernt. Entwurfsstatus
  bleibt sichtbar; konkrete Produktionsfragen stehen in production-open-items.md.

## Browser- und Layoutprüfung

Lokaler HTTP-Server, Playwright mit installiertem Chromium **149.0.7827.55**,
Windows-Systemfonts. Jede Seite bei 900 px Viewport-Höhe geprüft; Ganzseitenbilder
visuell kontrolliert. Mobile Startseiten zusätzlich in lesbaren Bildausschnitten geprüft.

| Seite | 1440 px | 375 px | 320 px |
| --- | --- | --- | --- |
| index.html | PASS | PASS | PASS |
| impressum.html | PASS | PASS | PASS |
| datenschutz.html | PASS | PASS | PASS |

Alle neun Kombinationen: kein horizontaler Overflow, keine abgeschnittenen
Überschriften, keine fehlenden Bilder, keine HTTP-Fehler der Seitenressourcen,
keine Console Errors oder JavaScript-Ausnahmen. Mobile Reihenfolge folgt der
Dokumentreihenfolge; das kleine Porträt steht nach dem Einführungstext.

Eine anfängliche Messung meldete bei eng gesetzten Überschriften Glyphenüberstand
über die Zeilenbox. Sichtbarer Overflow ist keine Abschneidung. Die korrigierte
Prüfung berücksichtigt tatsächliche Clipping-Vorfahren und Textgrenzen;
zusätzlich visuell bestätigt. Keine CSS-Kaschierung durch overflow:hidden.

## Links und Navigation

- Alle relativen Seiten-, CSS- und Bildpfade erreichbar; alle Fragmentziele vorhanden.
- Impressum, Datenschutz und E-Mail in jedem Seitenfooter; beide Legal-Seiten
  haben zusätzlich Rückverweise zur Startseite. aria-current markiert die aktive Seite.
- Keine en.html-Verweise, englischen hreflang-Angaben, leeren hrefs oder Dummy-URLs.
- GitHub-Profil: HTTP 200; Profil FHoffarth erreichbar.
- ORCID: HTTP 200. Öffentliche ORCID-API bestätigt Florian Hoffarth sowie die
  verknüpfte GND 138383448.
- DNB: 303 → 302 → 200, Ziel im DNB-Portal. Erste Python-Prüfung scheiterte an
  dessen Zertifikatsspeicher; curl mit Windows-Zertifikatsprüfung war erfolgreich.
  TLS-Prüfung wurde nicht ausgeschaltet.
- mailto-Adresse stimmt mit dem Entwurf überein. Zustellung UNKNOWN; keine E-Mail versendet.
- Projekttexte enthalten im freigegebenen Entwurf keine Produkt-URLs; keine erfunden.

## Accessibility

- lang=de, ein h1 pro Seite, folgende Ebenen h2/h3 ohne Sprünge.
- Semantische header/main/section/article/footer-Elemente und benannte Hero-Navigation.
- Skip-Link per Tab sichtbar und per Enter nutzbar; Fokus landet auf main#inhalt.
- Tab-Durchlauf aller Links: sichtbare Kontur, keine Fokusfallen.
- Porträt mit Alt-Text „Florian Hoffarth“ und expliziten Bildabmessungen.
- Berechnete Kontraste der sichtbaren Texte geprüft: keine Unterschreitung von
  4,5:1 für normalen bzw. 3:1 für großen Text. Dekorative aria-hidden-Pfeile und
  Trennzeichen sind ausgenommen.
- prefers-reduced-motion: reduce ergibt scroll-behavior: auto.
- Kein Screenreader-/Realgeräte-Test; vollständige WCAG-Konformität UNKNOWN.
  Safari, Firefox und abweichende Systemfonts sind nicht geprüft.

## Privacy und Produktionsgrenze

Bei allen neun Seitenaufrufen: **0 externe Ressourcenanfragen**, **0 Cookies**,
leerer Local-/Session-Storage, **0 Skripte**, **0 Formulare**, **0 Embeds**.
Nur HTML, gemeinsames CSS und auf der Startseite das lokale Porträt werden geladen.
Keine Analytics, Pixel, Telemetrie, externen Fonts oder Consent-Cookies.

Diese Aussagen betreffen den geprüften Website-Code. Künftige Hosting-Header,
Serverlogs, CDN- und E-Mail-Verarbeitung sind OPEN. Die Legal-Seiten sind
funktionsfähige Entwürfe, keine rechtliche Produktionsfreigabe.

## Review reproduzieren

1. Lokalen Server wie in README starten; jede HTML-Seite öffnen.
2. In den Entwicklertools 1440, 375 und 320 px einstellen und jede Seite durchscrollen.
3. Mit Tab/Enter Skip-Link, Inhaltslinks, Footer und Rücknavigation prüfen.
4. Netzwerk, Konsole und Speicher bei frischen Seitenaufrufen kontrollieren.
5. „Bewegung reduzieren“ emulieren; Textkontraste und Überschriften kontrollieren.
6. `git diff --check` vor dem Commit ausführen.

Lokale Messskripte, JSON-Protokolle und Screenshots liegen ausschließlich im
ignorierten work/-Verzeichnis des Checkouts; keine Testabhängigkeiten in der Website.
