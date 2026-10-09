## Hi, I'm Schnuecks 👋

3D printing enthusiast and homelab tinkerer from Germany. I build small self-hosted tools
for my own setup and share them when they might be useful to others too.

- 🖨️ **3D printing** on a Bambu Lab P2S and a Prusa Mini+
- 🏠 **Homelab & self-hosting**: my own services at home, running in Docker
- 🐍 Mostly **Python**, with a bit of Shell

If my projects are useful to you, you can buy me a coffee ☕ or send something via PayPal

<p>
  <a href="https://buymeacoffee.com/il6hhwtzr6"><img src="https://img.shields.io/badge/Buy_me_a_coffee-10_%E2%82%AC-FFDD00?logo=buymeacoffee&logoColor=black" alt="Buy me a coffee: 10 €"></a>
  <a href="https://buymeacoffee.com/il6hhwtzr6"><img src="https://img.shields.io/badge/Buy_me_a_coffee-25_%E2%82%AC-FFDD00?logo=buymeacoffee&logoColor=black" alt="Buy me a coffee: 25 €"></a>
  <a href="https://buymeacoffee.com/il6hhwtzr6"><img src="https://img.shields.io/badge/Buy_me_a_coffee-50_%E2%82%AC-FFDD00?logo=buymeacoffee&logoColor=black" alt="Buy me a coffee: 50 €"></a>
</p>

<p>
  <a href="https://paypal.me/Schnuecks/10EUR"><img src="https://img.shields.io/badge/PayPal-10_%E2%82%AC-00457C?logo=paypal&logoColor=white" alt="PayPal: 10 €"></a>
  <a href="https://paypal.me/Schnuecks/25EUR"><img src="https://img.shields.io/badge/PayPal-25_%E2%82%AC-00457C?logo=paypal&logoColor=white" alt="PayPal: 25 €"></a>
  <a href="https://paypal.me/Schnuecks/50EUR"><img src="https://img.shields.io/badge/PayPal-50_%E2%82%AC-00457C?logo=paypal&logoColor=white" alt="PayPal: 50 €"></a>
</p>

---

### <img src="assets/plateshelf-logo.svg" width="28" align="top" alt=""> [PlateShelf](https://github.com/Schnuecks/plateshelf) <img src="https://img.shields.io/badge/coming_soon-8A8A8A" alt="coming soon">

**A self-hosted archive for your 3D prints.** PlateShelf reads sliced files from Bambu Studio,
OrcaSlicer, PrusaSlicer, Cura and others and shows them as clearly as your slicer does:
plates with previews, print time, filament, costs and a 3D preview of the actual toolpaths.

- Direct import from **Bambu Lab**, **Prusa** (PrusaLink) and **Klipper** printers (Moonraker)
- **Print history** with statistics, notes per print and your own photos of the result
- User accounts with roles, daily backups, six languages, light and dark theme
- Runs as a single Docker container on a PC, NAS or Raspberry Pi

<p>
  <a href="https://github.com/Schnuecks/plateshelf"><img src="assets/plateshelf-overview.png" width="49%" alt="PlateShelf overview of all projects"></a>
  <a href="https://github.com/Schnuecks/plateshelf"><img src="assets/plateshelf-preview.png" width="49%" alt="PlateShelf 3D preview of the toolpaths"></a>
</p>

---

### <img src="assets/rdapi-logo.svg" width="28" align="top" alt=""> [RDAPI](https://github.com/Schnuecks/rdapi) <img src="https://img.shields.io/badge/public_beta-E4572E" alt="public beta">

**A lean self-hosted API server for the RustDesk app.** RDAPI adds what a household or a
small team needs on top of your own ID and relay server: signing in to the app, an address
book that follows you to every device, a device list and a history of incoming connections.

- **Address book** per user with tags, synchronised between all your devices
- **Device list** with online status and a **connection history**: who connected when and for how long
- Two-factor sign-in, **passkeys** and **single sign-on** via OpenID Connect
- Web interface in six languages, daily backups, one container with one SQLite file

Public beta: everything works, but a signed-in app can only connect once RustDesk releases
its ID server fix. More at [rdapi.app](https://rdapi.app).

<p>
  <a href="https://github.com/Schnuecks/rdapi"><img src="assets/rdapi-devices.png" width="49%" alt="RDAPI device list in the web interface"></a>
  <a href="https://github.com/Schnuecks/rdapi"><img src="assets/rdapi-history.png" width="49%" alt="RDAPI connection history"></a>
</p>

---

### <img src="assets/traefik-pihole-sync-logo.svg" width="28" align="top" alt=""> [traefik-pihole-sync](https://github.com/Schnuecks/traefik-pihole-sync)

**Traefik hostnames as local DNS records in Pi-hole v6.** Start a container with a `Host()`
rule and its name resolves on your network a minute later; remove it and the record goes
away again.

- **A, AAAA or CNAME records**, for one or several Pi-holes at once
- **Safe by design:** only deletes records it created itself, delayed deletion, dry-run mode
- Domain filter, quiet logs and a small non-root container for amd64 and arm64

---

<details>
<summary><b>🇩🇪 Auf Deutsch</b></summary>

<br>

**Hallo, ich bin Schnuecks!** 3D-Druck-Fan und Homelab-Bastler aus Deutschland. Ich baue
kleine selbstgehostete Werkzeuge für mein eigenes Setup und teile sie, wenn sie auch anderen
helfen können.

- 🖨️ **3D-Druck** mit einem Bambu Lab P2S und einem Prusa Mini+
- 🏠 **Homelab & Self-Hosting**: eigene Dienste zuhause, in Docker
- 🐍 Meistens **Python**, dazu etwas Shell

Wenn dir meine Projekte helfen, kannst du mir gern einen Kaffee ausgeben ☕ oder etwas per PayPal schicken – über die Knöpfe oben.

**[PlateShelf](https://github.com/Schnuecks/plateshelf)** *(demnächst)* ist ein selbstgehostetes Archiv für
deine 3D-Drucke: Platten mit Vorschaubildern, Druckzeit, Filament, Kosten und eine 3D-Vorschau
der Druckbahnen, dazu Direktimport von Bambu-, Prusa- und Klipper-Druckern, Druckverlauf mit
Statistik, Fotos vom fertigen Druck und sechs Sprachen – in einem einzigen Docker-Container.

**[RDAPI](https://github.com/Schnuecks/rdapi)** *(öffentliche Beta)* ist ein schlanker, selbstgehosteter API-Server
für die RustDesk-App: Anmeldung in der App, ein Adressbuch, das dir auf jedes Gerät folgt,
eine Geräteliste und ein Verlauf eingehender Verbindungen, dazu Zwei-Faktor-Anmeldung,
Passkeys, Single Sign-on und eine Weboberfläche in sechs Sprachen – ein Container, eine
SQLite-Datei.

**[traefik-pihole-sync](https://github.com/Schnuecks/traefik-pihole-sync)** trägt die
Hostnamen deiner Traefik-Router automatisch als lokale DNS-Einträge in Pi-hole v6 ein: als
A-, AAAA- oder CNAME-Eintrag, für einen oder mehrere Pi-holes. Es löscht nur Einträge, die es
selbst angelegt hat, und hat einen Probelauf-Modus.

</details>
