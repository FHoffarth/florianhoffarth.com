# Produktionscheckliste

Stand: 2026-09-05. GitHub Pages ist als Hostingdienst ausgewählt, aber noch nicht
aktiviert. Diese Checkliste trennt bestätigte Tatsachen von Prüfungen am späteren
Live-System und konkreten Freigabeblockern.

## RESOLVED

- **Anbieter- und Postanschrift:** Florian Hoffarth, Ringstr. 48, 64807 Dieburg,
  Deutschland, ist zur Veröffentlichung freigegeben und in Impressum sowie
  Datenschutzerklärung eingetragen.
- **Kontakt:** Die bereits veröffentlichte E-Mail-Adresse
  `florian.hoffarth1981@gmail.com` ist in beiden Legal-Seiten angegeben.
- **Art der Website:** Persönliches berufliches Profil und Evidence Layer ohne Shop,
  SaaS-Angebot, Arbeitgeberfunktion, journalistisch-redaktionellen Nachrichtendienst,
  Registrierung, Werbung oder Kontaktformular. Es werden keine nicht belegten
  Register-, Unternehmens-, Kammer-, Steuer-, Lizenz- oder Aufsichtsangaben gemacht.
- **Porträt:** Florian Hoffarth hat bestätigt, dass es sein eigenes Bild ist, er die
  Veröffentlichungsrechte hält und die Veröffentlichung auf dieser Website beabsichtigt.
- **Technische Datenschutzarchitektur:** Statisches HTML/CSS, lokales Porträt,
  Systemschriftarten, kein JavaScript, keine Analytics, kein Tracking, keine vom
  Website-Code gesetzten Cookies, keine Formulare, kein Login und keine Drittanbieter-
  Embeds. Externe Ziele werden nur über gewöhnliche Links aufgerufen.
- **Hostingauswahl:** GitHub Pages ist ausgewählt. GitHub dokumentiert, dass beim
  Besuch einer Pages-Website Besucher-IP-Adressen zu Sicherheitszwecken protokolliert
  und gespeichert werden, unabhängig von einer Anmeldung bei GitHub. Diese Information
  ist im Datenschutztext enthalten.
- **Unbelegte Hostingdetails:** Es werden keine konkreten Log-Speicherfristen,
  Serverstandorte, Unterauftragnehmer, Vertragsdetails oder Mechanismen internationaler
  Datenübermittlung behauptet.

## VERIFY AFTER ACTIVATION

- **GitHub-Pages-Auslieferung:** Aktivierung und tatsächlich veröffentlichte Dateien,
  Pfade, Fehlerseiten und Erreichbarkeit aller drei Seiten prüfen.
- **Custom Domain und DNS:** Ziel-Domain, DNS-Einträge und Schutz vor Fehlzuordnung
  anhand der aktiven Konfiguration prüfen.
- **HTTPS:** Zertifikat, HTTPS-Erzwingung und Mixed Content am Live-System prüfen.
- **Weiterleitungen:** `http`/`https`, `www`/Apex und GitHub-Pages-Ziel auf eindeutige,
  funktionierende Weiterleitungen prüfen.
- **Response-Header:** Tatsächliche Sicherheits-, Caching- und Content-Type-Header
  dokumentieren und bewerten.
- **Live-Verhalten:** Netzwerkverkehr, externe Ressourcen, Cookies, Web Storage,
  Konsolenfehler und Formular-/Skriptfreiheit erneut auf der Produktions-URL prüfen.
- **Links:** Interne Navigation, Fragmentziele, E-Mail-Link und externe Ziele von der
  Produktions-URL aus prüfen.
- **Finaler Datenschutz-/Legal-Abgleich:** Den Text gegen die tatsächlich aktive
  Pages-, Domain- und E-Mail-Konfiguration prüfen und nur nachgewiesene Abweichungen
  korrigieren.

## BLOCKER

- **Rechtsgrundlagen und Pflichtinformationen:** Vor öffentlicher Freigabe muss eine
  qualifizierte rechtliche Prüfung bestimmen, welche Rechtsgrundlagen und ergänzenden
  Pflichtinformationen für die GitHub-Pages-Auslieferung und die Bearbeitung von
  E-Mail-Anfragen gelten. Diese Angaben sind im aktuellen Kandidaten bewusst nicht
  geraten. Optional nicht dokumentierte Hostingdetails sind für sich genommen kein
  Blocker; die fehlende rechtliche Bewertung der tatsächlich stattfindenden
  Verarbeitungen ist der konkrete offene Freigabepunkt.

## Quellen für die Abschlussprüfung

- [GitHub Pages: Data collection](https://docs.github.com/en/pages/getting-started-with-github-pages/what-is-github-pages#data-collection)
- [§ 5 DDG](https://www.gesetze-im-internet.de/ddg/__5.html)
- [DSGVO](https://eur-lex.europa.eu/legal-content/DE/TXT/?uri=CELEX:02016R0679-20160504)

Die Quellen und diese technische Bestandsaufnahme sind keine Erklärung rechtlicher
Gewissheit. Es wurden weder GitHub Pages aktiviert noch CNAME-, DNS-, Deployment-
oder Merge-Änderungen vorgenommen.
