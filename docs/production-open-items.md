# Vor einer Veröffentlichung zu klären

Die technische V1 ist ein Review-Stand. Impressum und Datenschutz sind eigenständige,
ausdrücklich als Entwurf gekennzeichnete Seiten mit `noindex`. Das ersetzt keine
vollständigen Anbieter- und Datenschutzangaben und verhindert keinen öffentlichen Zugriff.

## Impressum — OPEN

- Veröffentlichungsfähige, vollständige Anschrift des Verantwortlichen bestätigen.
  Die private Anschrift aus dem Export wurde auch aus dessen sichtbaren TODOs entfernt.
- Einordnung des Angebots und daraus folgende Pflichtangaben prüfen, einschließlich
  Anwendbarkeit von § 5 DDG und § 18 MStV. Keine geschäftsmäßige oder rein private
  Einordnung vorweggenommen; keine Kammer, Register- oder Steuerdaten erfunden.
- Erforderliche Möglichkeiten unmittelbarer Kontaktaufnahme klären; keine pauschale
  Behauptung, dass eine E-Mail-Adresse stets genügt. Telefonnummer nur nach Freigabe.
- Nutzungsrechte des Porträts für die öffentliche Website bestätigen. Das Foto stammt
  aus der bereitgestellten Design-ZIP; eine Lizenz wurde damit nicht nachgewiesen.

## Datenschutz — OPEN

- Vollständige Verantwortlichenangaben nachtragen.
- Tatsächliche E-Mail-Verarbeitung klären: Dienstanbieter, Empfänger, Zwecke,
  passende Rechtsgrundlagen, Speicher-/Löschpraxis, gegebenenfalls Drittlandtransfers.
  Aus der Gmail-Adresse werden keine vertraglichen Details abgeleitet.
- Informationspflichten anhand aller tatsächlichen Verarbeitungsvorgänge finalisieren;
  Entwurfshinweise erst nach vollständiger Prüfung ersetzen.

## Hosting — OPEN / UNKNOWN

- Anbieter, Vertragspartner, Serverstandorte und gegebenenfalls CDN festlegen.
- Zugriffsdaten/Logfelder, Zwecke, Rechtsgrundlage und konkrete Speicherdauer erheben.
- Auftragsverarbeitung, Unterauftragnehmer und mögliche Drittlandtransfers prüfen.
- Tatsächliche Response-Header, TLS, Caching, Fehlerseiten und Weiterleitungen prüfen.
- Nach Auswahl sicherstellen, dass die Plattform keine zusätzlichen Skripte,
  Analytics, Cookies, Telemetrie oder sonstigen externen Ressourcen einschleust.
- Nur die drei HTML-Dateien, styles.css und assets/ als öffentliche Site verwenden;
  Review-Dokumentation und lokale Arbeitsdateien gehören nicht ins öffentliche Webroot.
- Domain/DNS-Zustand und bestehende Hosting-Integrationen sind UNKNOWN.
  Diese Implementierung hat keine entsprechende Konfiguration geändert.

## Quellen für die rechtliche Abschlussprüfung

- [§ 5 DDG](https://www.gesetze-im-internet.de/ddg/__5.html)
- [DSGVO, insbesondere Art. 13 und 15–21 sowie 77](https://eur-lex.europa.eu/legal-content/DE/TXT/?uri=CELEX:32016R0679)

Die Quellen ersetzen nicht die Erhebung der tatsächlichen Betriebsabläufe.
Keine Freigabe für Production allein durch technischen Test oder `noindex`.
