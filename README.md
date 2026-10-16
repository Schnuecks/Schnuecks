## Hi, I'm Schnuecks 👋

**English** · [Deutsch](https://github.com/Schnuecks/Schnuecks/blob/main/README.de.md)

3D printing enthusiast and homelab tinkerer from Germany. I build small self-hosted tools
for my own setup and share them when they might be useful to others too.

- 🖨️ **3D printing** on a Bambu Lab P2S and a Prusa Mini+
- 🏠 **Homelab & self-hosting**: my own services at home, running in Docker
- 🐍 Mostly **Python**, with a bit of Shell
- 🌐 All my projects at a glance: **[schnuecks.dev](https://schnuecks.dev)**

AI coding assistants are part of my workflow: they help me draft code, tests and documentation.
What gets built, how it behaves and what gets released is my decision, and every release is
tested on my own hardware first.

Security is part of that, not an afterthought. Every project runs its test suite, a container
scan (Trivy) and Dependabot on each change; the web apps are also scanned with OWASP ZAP.
Before going public, each project gets a security review: findings are reproduced with a test,
fixed, and the fix is checked again – you can follow it in the changelogs. Found something?
Every repository has a [security policy](https://github.com/Schnuecks/rdapi/security/policy)
for reporting it privately.

If my projects are useful to you, you can buy me a coffee ☕ on Ko-fi

<p>
  <a href="https://ko-fi.com/schnuecks"><img src="https://ko-fi.com/img/githubbutton_sm.svg" alt="Support me on Ko-fi"></a>
</p>

---

### <img src="assets/plateshelf-logo.svg" width="28" align="top" alt=""> [PlateShelf](https://github.com/Schnuecks/plateshelf) <img src="https://img.shields.io/badge/stable-2E7D32" alt="stable">

**A self-hosted archive for your 3D prints.** PlateShelf reads sliced files from Bambu Studio,
OrcaSlicer, PrusaSlicer, Cura and others and shows them as clearly as your slicer does:
plates with previews, print time, filament, costs and a 3D preview of the actual toolpaths.

- Direct import from **Bambu Lab**, **Prusa** (PrusaLink), **Klipper** (Moonraker) and **OctoPrint** printers
- **Print history** with statistics, notes per print and your own photos of the result
- User accounts with roles, passkeys, single sign-on, daily backups, six languages, light and dark theme
- Runs as a single Docker container on a PC, NAS or Raspberry Pi

<p>
  <a href="https://github.com/Schnuecks/plateshelf"><img src="assets/plateshelf-overview.png" width="49%" alt="PlateShelf overview of all projects"></a>
  <a href="https://github.com/Schnuecks/plateshelf"><img src="assets/plateshelf-preview.png" width="49%" alt="PlateShelf 3D preview of the toolpaths"></a>
</p>

---

### <img src="assets/mailreports-logo.svg" width="28" align="top" alt=""> [mailreports](https://github.com/Schnuecks/mailreports) <img src="https://img.shields.io/badge/stable-2E7D32" alt="stable">

**DMARC and TLS reports in plain words.** mailreports fetches the daily DMARC and SMTP TLS
reports for your domains from a mailbox and explains them: who sent email in your name,
whether it was genuine and what the receiving servers did with it – instead of XML and
result codes.

- **Every report record explained**, senders classified as your own servers, services, forwarders or unknown, with reverse DNS and network
- **DNS check** for DMARC, SPF, DKIM, MTA-STS and TLS-RPT, and a recommendation when the policy can be tightened
- **Notifications** via Pushover, ntfy, webhook or email, plus a weekly summary
- Passkeys, single sign-on, six languages; one container, one SQLite file. More at [mailreports.app](https://mailreports.app)

<p>
  <a href="https://github.com/Schnuecks/mailreports"><img src="assets/mailreports-overview.png" width="49%" alt="mailreports overview with the DMARC pass rate of two domains"></a>
  <a href="https://github.com/Schnuecks/mailreports"><img src="assets/mailreports-report.png" width="49%" alt="mailreports explaining a DMARC report record by record"></a>
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

### <img src="assets/print-roulette-logo.svg" width="28" align="top" alt=""> [Print Roulette](https://github.com/Schnuecks/print-roulette) <img src="https://img.shields.io/badge/stable-2E7D32" alt="stable">

**Spin the wheel and discover a random 3D print.** Print Roulette picks a model from
MakerWorld, Printables, Cults3D or Thingiverse and links straight to its page, for the
evenings when you want to print something but don't know what.

- **Prize wheel** in the platform colours: spin for a random platform or roll on one directly
- **Preview image, title and creator**, filters for free models and for hiding NSFW content
- **No database, no login, no tracking**, six languages, light and dark mode
- A small container with no dependencies beyond the Python standard library

<p>
  <a href="https://github.com/Schnuecks/print-roulette"><img src="assets/print-roulette-desktop.png" width="64%" alt="Print Roulette with the prize wheel, a result and the history"></a>
  <a href="https://github.com/Schnuecks/print-roulette"><img src="assets/print-roulette-mobile.png" width="31%" alt="Print Roulette on a phone in light mode"></a>
</p>

---

### <img src="assets/traefik-pihole-sync-logo.svg" width="28" align="top" alt=""> [traefik-pihole-sync](https://github.com/Schnuecks/traefik-pihole-sync) <img src="https://img.shields.io/badge/stable-2E7D32" alt="stable">

**Traefik hostnames as local DNS records in Pi-hole v6.** Start a container with a `Host()`
rule and its name resolves on your network a minute later; remove it and the record goes
away again.

- **A, AAAA or CNAME records**, for one or several Pi-holes at once
- **Safe by design:** only deletes records it created itself, delayed deletion, dry-run mode
- Domain filter, quiet logs and a small non-root container for amd64 and arm64
