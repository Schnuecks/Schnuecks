## Hallo, ich bin Schnuecks 👋

[English](https://github.com/Schnuecks) · **Deutsch**

3D-Druck-Fan und Homelab-Bastler aus Deutschland. Ich baue kleine selbstgehostete Werkzeuge
für mein eigenes Setup und teile sie, wenn sie auch anderen helfen können.

- 🖨️ **3D-Druck** mit einem Bambu Lab P2S und einem Prusa Mini+
- 🏠 **Homelab & Self-Hosting**: eigene Dienste zuhause, in Docker
- 🐍 Meistens **Python**, dazu etwas Shell
- 🌐 Alle Projekte auf einen Blick: **[schnuecks.dev/de](https://schnuecks.dev/de/)**

KI-Assistenten gehören zu meinem Werkzeugkasten: Sie helfen mir beim Entwurf von Code, Tests und
Dokumentation. Was gebaut wird, wie es sich verhält und was veröffentlicht wird, entscheide ich,
und jedes Release läuft vorher auf meiner eigenen Hardware.

Sicherheit gehört dazu und kommt nicht hinterher. Jedes Projekt durchläuft bei jeder Änderung
seine Tests, einen Container-Scan (Trivy) und Dependabot; die Web-Apps werden zusätzlich mit
OWASP ZAP gescannt. Vor der Veröffentlichung bekommt jedes Projekt einen Sicherheits-Review:
Funde werden mit einem Test nachgestellt, behoben und danach erneut geprüft – nachzulesen in den
Changelogs. Etwas gefunden? Jedes Repository hat eine Sicherheitsrichtlinie, um es vertraulich
zu melden.

Wenn dir meine Projekte helfen, kannst du mir gern auf Ko-fi einen Kaffee ausgeben ☕

<p>
  <a href="https://ko-fi.com/schnuecks"><img src="https://ko-fi.com/img/githubbutton_sm.svg" alt="Unterstütze mich auf Ko-fi"></a>
</p>

---

### <img src="assets/plateshelf-logo.svg" width="28" align="top" alt=""> [PlateShelf](https://github.com/Schnuecks/plateshelf) <img src="https://img.shields.io/badge/stabil-2E7D32" alt="stabil">

**Ein selbstgehostetes Archiv für deine 3D-Drucke.** PlateShelf liest geslicte Dateien aus
Bambu Studio, OrcaSlicer, PrusaSlicer, Cura und anderen und zeigt sie so übersichtlich wie dein
Slicer: Platten mit Vorschau, Druckzeit, Filament, Kosten und eine 3D-Vorschau der echten
Druckbahnen.

- Direktimport von **Bambu-Lab-**, **Prusa-** (PrusaLink), **Klipper-** (Moonraker) und **OctoPrint-**Druckern
- **Druckverlauf** mit Statistik, Notizen je Druck und eigenen Fotos vom fertigen Druck
- Benutzerkonten mit Rollen, Passkeys, Single Sign-on, tägliche Sicherungen, sechs Sprachen, helles und dunkles Design
- Läuft als ein einziger Docker-Container auf PC, NAS oder Raspberry Pi

<p>
  <a href="https://github.com/Schnuecks/plateshelf"><img src="assets/plateshelf-overview.png" width="49%" alt="PlateShelf-Übersicht aller Projekte"></a>
  <a href="https://github.com/Schnuecks/plateshelf"><img src="assets/plateshelf-preview.png" width="49%" alt="PlateShelf mit der 3D-Vorschau der Druckbahnen"></a>
</p>

---

### <img src="assets/mailreports-logo.svg" width="28" align="top" alt=""> [mailreports](https://github.com/Schnuecks/mailreports) <img src="https://img.shields.io/badge/stabil-2E7D32" alt="stabil">

**DMARC- und TLS-Berichte im Klartext.** mailreports holt die täglichen DMARC- und
SMTP-TLS-Berichte deiner Domains aus einem Postfach und erklärt sie: wer in deinem Namen
E-Mails versendet hat, ob sie echt waren und wie die empfangenden Server damit verfahren sind –
statt XML und Fehlercodes.

- **Jeder Berichtseintrag erklärt**, Absender eingeordnet als eigene Server, beauftragte Dienste, Weiterleitungen oder Unbekannte, mit Reverse-DNS und Netz
- **DNS-Prüfung** für DMARC, SPF, DKIM, MTA-STS und TLS-RPT und eine Empfehlung, wann die Richtlinie strenger werden kann
- **Benachrichtigungen** per Pushover, ntfy, Webhook oder E-Mail, dazu eine Wochenübersicht
- Passkeys, Single Sign-on, sechs Sprachen; ein Container, eine SQLite-Datei. Mehr auf [mailreports.app](https://mailreports.app/de/)

<p>
  <a href="https://github.com/Schnuecks/mailreports"><img src="assets/mailreports-overview.png" width="49%" alt="mailreports-Übersicht mit der DMARC-Bestehensquote zweier Domains"></a>
  <a href="https://github.com/Schnuecks/mailreports"><img src="assets/mailreports-report.png" width="49%" alt="mailreports erklärt einen DMARC-Bericht Eintrag für Eintrag"></a>
</p>

---

### <img src="assets/rdapi-logo.svg" width="28" align="top" alt=""> [RDAPI](https://github.com/Schnuecks/rdapi) <img src="https://img.shields.io/badge/%C3%B6ffentliche_Beta-E4572E" alt="öffentliche Beta">

**Ein schlanker, selbstgehosteter API-Server für die RustDesk-App.** RDAPI ergänzt deinen
eigenen ID- und Relay-Server um das, was ein Haushalt oder ein kleines Team braucht: Anmeldung
in der App, ein Adressbuch, das dir auf jedes Gerät folgt, eine Geräteliste und einen Verlauf
eingehender Verbindungen.

- **Adressbuch** pro Benutzer mit Tags, auf allen deinen Geräten gleich
- **Geräteliste** mit Online-Status und **Verbindungsverlauf**: wer sich wann und wie lange verbunden hat
- Zwei-Faktor-Anmeldung, **Passkeys** und **Single Sign-on** über OpenID Connect
- Weboberfläche in sechs Sprachen, tägliche Sicherungen, ein Container mit einer SQLite-Datei

Öffentliche Beta: Alles funktioniert, aber eine angemeldete App kann sich erst verbinden, wenn
RustDesk die Korrektur für seinen ID-Server veröffentlicht. Mehr auf [rdapi.app](https://rdapi.app).

<p>
  <a href="https://github.com/Schnuecks/rdapi"><img src="assets/rdapi-devices.png" width="49%" alt="RDAPI-Geräteliste in der Weboberfläche"></a>
  <a href="https://github.com/Schnuecks/rdapi"><img src="assets/rdapi-history.png" width="49%" alt="RDAPI-Verbindungsverlauf"></a>
</p>

---

### <img src="assets/print-roulette-logo.svg" width="28" align="top" alt=""> [Print Roulette](https://github.com/Schnuecks/print-roulette) <img src="https://img.shields.io/badge/stabil-2E7D32" alt="stabil">

**Am Rad drehen und einen zufälligen 3D-Druck entdecken.** Print Roulette wählt ein Modell von
MakerWorld, Printables, Cults3D oder Thingiverse und verlinkt direkt auf dessen Seite – für die
Abende, an denen du etwas drucken willst, aber nicht weißt, was.

- **Glücksrad** in den Farben der Plattformen: für eine zufällige Plattform drehen oder direkt auf einer würfeln
- **Vorschaubild, Titel und Ersteller**, Filter für kostenlose Modelle und gegen NSFW-Inhalte
- **Keine Datenbank, keine Anmeldung, kein Tracking**, sechs Sprachen, helles und dunkles Design
- Ein kleiner Container ohne Abhängigkeiten außer der Python-Standardbibliothek

<p>
  <a href="https://github.com/Schnuecks/print-roulette"><img src="assets/print-roulette-desktop.png" width="64%" alt="Print Roulette mit Glücksrad, Ergebnis und Verlauf"></a>
  <a href="https://github.com/Schnuecks/print-roulette"><img src="assets/print-roulette-mobile.png" width="31%" alt="Print Roulette auf dem Handy im hellen Design"></a>
</p>

---

### <img src="assets/traefik-pihole-sync-logo.svg" width="28" align="top" alt=""> [traefik-pihole-sync](https://github.com/Schnuecks/traefik-pihole-sync) <img src="https://img.shields.io/badge/stabil-2E7D32" alt="stabil">

**Traefik-Hostnamen als lokale DNS-Einträge in Pi-hole v6.** Starte einen Container mit einer
`Host()`-Regel, und eine Minute später löst sein Name im ganzen Netz auf; entfernst du ihn,
verschwindet auch der Eintrag.

- **A-, AAAA- oder CNAME-Einträge**, für einen oder mehrere Pi-holes gleichzeitig
- **Sicher gebaut:** löscht nur Einträge, die es selbst angelegt hat, verzögertes Löschen, Probelauf-Modus
- Domainfilter, ruhige Logs und ein kleiner Container ohne Root-Rechte für amd64 und arm64
