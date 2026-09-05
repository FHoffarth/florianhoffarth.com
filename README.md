# florianhoffarth.com

Statische persönliche Website mit der Positionierung
**Kommunalverwaltung · Führung · Digitalisierung · Kommunikation**.
Die V1 übernimmt den freigegebenen Claude-Design-Entwurf aus der bereitgestellten ZIP.

## Struktur

```text
index.html                      Beruflicher Werdegang, Projekte, Forschung, Kontakt
impressum.html                  Anbieterangaben, ausdrücklich noch Entwurf
datenschutz.html                Datenschutzhinweise, ausdrücklich noch Entwurf
styles.css                      Gemeinsames Layout und responsive Regeln
assets/portrait.png             Lokales Porträt aus dem Entwurf
docs/production-open-items.md   Vor Veröffentlichung zu klärende Angaben
docs/verification.md            Prüfungen, Designabgleich und Grenzen
```

## Lokal ansehen

Kein Build, Paketmanager oder JavaScript erforderlich. Die HTML-Dateien können
direkt im Browser geöffnet werden. Für eine HTTP-Prüfung im Repository:

```sh
python -m http.server 8000 --bind 127.0.0.1
```

Danach `http://127.0.0.1:8000/index.html` im Browser öffnen. Der Server ist nur für
die lokale Prüfung vorgesehen; mit Strg+C beenden.

## Technische Grenzen

- HTML und CSS, Systemschriftarten und ein lokales PNG; keine Abhängigkeiten.
- Kein Formular-Backend, keine Cookies, kein Tracking und keine externen Embeds.
- Externe Profile sind normale Links. E-Mail öffnet das lokale E-Mail-Programm.
- Ausschließlich deutsche V1; kein Sprachumschalter und keine englischen Verweise.
- Keine Hosting-, Domain-, DNS-, GitHub-Pages- oder Deployment-Konfiguration.

Impressum und Datenschutz sind vor einer Veröffentlichung zu vervollständigen.
Die [offenen Produktionsangaben](docs/production-open-items.md) und der
[Prüfbericht](docs/verification.md) gehören zum Review. `noindex` ist kein Zugriffsschutz.
