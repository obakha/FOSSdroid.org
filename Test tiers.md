## 🛡️ Tiered Degoogling Roadmap 

---

### **1. Light Tier 🐣: "Basic Hygiene"**  
*For minimalists dipping into privacy*  

**Threat Model**: Reduce surface tracking from ads/OEM bloat.  

**Key Actions**:  
- Remove preinstalled apps via [Universal Android Debloater](https://github.com/0x192/universal-android-debloater)  
- Replace Chrome with [Privacy Browser](https://f-droid.org/packages/com.stoutner.privacybrowser.standard/)  
- Use [Aurora Store](https://f-droid.org/fr/packages/com.aurora.store/) (anonymous mode)  

**Tools**:  
| Category | FOSS Alternative |  
|----------|------------------|  
| Search | [DuckDuckGo](https://duckduckgo.com/) |  
| Email | [ProtonMail](https://proton.me/mail) |  
| Drive | [Proton Drive](https://proton.me/drive) |  

**Warnings**:  
- Google Services Framework (GSF) still active  
- Location leaks via Wi-Fi/Mobile networks  

---

### **2. Normal Tier 🛡️: "Balanced Defense"**  
*For privacy-conscious daily drivers*  

**Threat Model**: Block telemetry, ads, and data brokers.  

**Key Actions**:  
- Install [CalyxOS](https://calyxos.org/) with MicroG toggle  
- Enable [Hagezi Normal DNS](https://github.com/hagezi/dns-blocklists)  
- Migrate to FOSS apps via [Accrescent](https://accrescent.app/)  

**Tools**:  
| Category | FOSS Alternative |  
|----------|------------------|  
| Browser | [Vanadium](https://grapheneos.org/usage#vanadium) (GrapheneOS) |  
| Maps | [Organic Maps](https://organicmaps.app/) |  
| Docs | [Cryptpad](https://cryptpad.fr/) |  

**Warnings**:  
- Banking apps may require [Shelter](https://github.com/PeterCxy/Shelter) isolation  
- WearOS/Fitbit integration breaks  

---

### **3. Pro Tier 🔥: "Zero-Trust Mobile"**  
*For tech-savvy users ditching Google*  

**Threat Model**: Eliminate Google dependencies, defeat fingerprinting.  

**Key Actions**:  
- Install [GrapheneOS](https://grapheneos.org/) (Pixel only)  
- Block Google APIs via [RethinkDNS](https://github.com/celzero/rethink-app)  
- Self-host with [Nextcloud](https://nextcloud.com/)  

**Tools**:  
| Category | FOSS Alternative |  
|----------|------------------|  
| App Store | [Obtainium](https://github.com/ImranR98/Obtainium) |  
| Search | [Leta](https://leta.mullvad.net/) (Mullvad) |  
| Cloud | [Tresorit](https://tresorit.com/) (E2EE) |  

**Warnings**:  
- No Google Pay/WearOS  
- Camera quality loss (no HDR+)  

---

### **4. Pro++ Tier ☢️: "Fortress Mode"**  
*For journalists/activists*  

**Threat Model**: Maximum anonymity, anti-surveillance.  

**Key Actions**:  
- **Baseband Removal**: Disable cellular modem (Wi-Fi only)  
- **Network Hardening**: Tor → VPN → Tor chains via [Orbot](https://guardianproject.info/apps/org.torproject.android/)  
- **Air-Gapped Backups**: Use Faraday bags for offline storage  

**Tools**:  
| Category | FOSS Alternative |  
|----------|------------------|  
| Comms | [Briar](https://briarproject.org/) (offline mesh) |  
| OS | [GraphenOS](https://grapheneos.org/install) |  
| Browsing | [Tor Browser](https://www.torproject.org/download/) |  

**Warnings**:  
- 40%+ app incompatibility  
- High maintenance (weekly log audits)  

---

## 🔧 **The Hated One's Toolkit**  
*Essential Apps & Configs*  

### **Google Alternatives**  
| Service | Replacement |  
|---------|-------------|  
| Play Store | Aurora Store (sandboxed) + [Accrescent](https://accrescent.app/) |  
| Chrome | Vanadium (GrapheneOS) / Mullvad Browser |  
| Docs | LibreOffice + Cryptpad |  
| Maps | OSMAnd (offline) |  

### **Advanced Privacy Tools**  
- [CanvasBlocker](https://addons.mozilla.org/en-US/firefox/addon/canvasblocker/): Spoof GPU/OS fingerprints  
- [NetGuard](https://github.com/M66B/NetGuard): Block apps from phoning home  
- [Syncthing](https://syncthing.net/): Google Drive replacement  

---

## ⚠️ **Critical Warnings**  
1. **Banking Apps**:  
   - Isolate in Shelter work profile  
   - Use Aurora Store *anonymous mode*  
2. **Location Tracking**:  
   - Disable Wi-Fi/Bluetooth scanning  
   - Set `captive_portal_https_url` to non-Google endpoint  
3. **App Sources**:  
   - Avoid APKMirror/APKPure (use [Accrescent](https://accrescent.app/) or F-Droid)  

---

## 📜 **Implementation Roadmap**  
1. **Week 1**: Light tier setup (debloat + browser swap)  
2. **Month 1**: Normal tier migration (CalyxOS + DNS filtering)  
3. **Month 3**: Pro tier transition (GrapheneOS + self-hosting)  
4. **Ongoing**: Pro++ hardening (air-gapping, Tor-only)  

---

**Resources**:  
- [The Hated One's Video](https://yewtu.be/watch?v=nnLSWBBQSEU&list=PLR_ghQEN2SgBOLJaDomLoK95Ay_xV5aZV&index=0)  
- [LINDDUN Framework](https://www.linddun.org/)  
- [GrapheneOS Install Guide](https://grapheneos.org/install)  
