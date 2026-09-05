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
- **Rechtsgrundlage der Auslieferung:** Art. 6 Abs. 1 lit. f DSGVO für die vom
  Websitebetreiber veranlasste erforderliche Verarbeitung zur sicheren, zuverlässigen
  und missbrauchsresistenten Bereitstellung. Abwägung für diesen Kandidaten: gewöhnliche
  technische Auslieferung ist für den freiwilligen Seitenaufruf erforderlich;
  der Website-Code fügt keine Analyse, Profile, Tracker oder Embeds hinzu.
  Dies betrifft das persönliche Webangebot, keine behördliche Aufgabenerfüllung.
  Die Aussage erstreckt sich nicht pauschal auf alle eigenen Verarbeitungen GitHubs.
- **Rechtsgrundlagen der E-Mail-Kommunikation:** Art. 6 Abs. 1 lit. b DSGVO nur,
  soweit für einen Vertrag mit der anfragenden Person oder vorvertragliche Maßnahmen
  auf deren Anfrage erforderlich; sonst lit. f für die Beantwortung gerichteter
  Korrespondenz. Die vom Nutzer vorgegebene Aufbewahrung nach Erforderlichkeit,
  gesetzlichen Pflichten und notwendiger Rechtsverteidigung ist aufgenommen.
- **Speicherkriterien und internationale Verarbeitung:** GitHubs allgemeine
  Speichermaßstäbe sind als solche wiedergegeben, nicht als konkrete Pages-Logfrist.
  Das General Privacy Statement (wirksam seit 27.04.2026) beschreibt Verarbeitung
  in den USA und weiteren Ländern sowie SCCs und EU-U.S. DPF. Der verlinkte Hinweis
  ordnet keinen einzelnen Mechanismus speziell den Pages-Besucherlogs zu.
  Keine erfundenen Standorte, Unterauftragnehmer oder Vertragsdetails.
- **Art.-13-Informationen für die beschriebenen Vorgänge:** Name/Anschrift/Kontakt,
  Zwecke, Rechtsgrundlagen, berechtigte Interessen, beteiligter Hostinganbieter und
  Empfängerkategorie Maildienstanbieter, Speichermaßstäbe, GitHubs internationale
  Hinweise samt Quellen, Betroffenenrechte und Beschwerderecht sind enthalten.
  Freiwilligkeit und Folgen fehlender erforderlicher Angaben sind erläutert.
  Der Website-Code enthält keine automatisierte Entscheidungsfindung; eine
  Einwilligung wird für die hier beschriebenen Vorgänge nicht als Grundlage verwendet.
  Unbestätigte Gmail-Verträge oder spezifische Google-Transferdetails werden nicht
  unterstellt. Die allgemeinen GitHub-Angaben belegen keine Log-spezifische Konfiguration.

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

Kein konkreter verbleibender Offenlegungsblocker für die beschriebenen Vorgänge
aus den geprüften Quellen und bekannten Tatsachen identifiziert. Der pauschale
Prozessvorbehalt einer „qualifizierten rechtlichen Prüfung“ entfällt.
Art. 13 erlaubt Empfängerkategorien und, wenn eine feste Dauer nicht angegeben werden
kann, Speicherkriterien. Eine nicht veröffentlichte Pages-Logfrist ist daher allein
kein Blocker. Die Quellen ersetzen keine Garantie rechtlicher Vollständigkeit für
abweichende tatsächliche Verarbeitungen. Zeigt der Live-Abgleich zusätzliche
Verarbeitungen oder unzutreffende Angaben, ist die konkrete Abweichung zu beheben.

## Quellen für die Abschlussprüfung

- [GitHub Pages: Data collection](https://docs.github.com/en/pages/getting-started-with-github-pages/what-is-github-pages#data-collection)
- [GitHub General Privacy Statement: Speicherung, internationale Verarbeitung und Garantien](https://docs.github.com/en/site-policy/privacy-policies/github-general-privacy-statement)
- [DSGVO, insbesondere Art. 6 und Art. 13](https://eur-lex.europa.eu/legal-content/DE/TXT/?uri=CELEX:02016R0679-20160504)

Die Quellen und diese technische Bestandsaufnahme sind keine Erklärung rechtlicher
Gewissheit. Es wurden weder GitHub Pages aktiviert noch CNAME-, DNS-, Deployment-
oder Merge-Änderungen vorgenommen.
