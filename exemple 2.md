## Tiered Degoogling Roadmap  

### 1. 🐣 Light Tier: "Basic Hygiene"  
*For minimalists*  

**Threat Model**: Reduce ads/OEM tracking  
**Tools**:  
- [Universal Android Debloater](https://github.com/0x192/universal-android-debloater)  
- [Mullvad Browser](https://mullvad.net/en/browser)  
- [Aurora Store](https://auroraoss.com/) (Anonymous Mode)  

**Warnings**:  
- Google Services Framework (GSF) still active  
- Location leaks via Wi-Fi  

---

### 2. 🛡️ Normal Tier: "Balanced Defense"  
*For daily drivers*  

**Threat Model**: Block telemetry/data brokers  
**Tools**:  
- [CalyxOS](https://calyxos.org/) + MicroG toggle  
- [Hagezi Normal DNS](https://github.com/hagezi/dns-blocklists)  
- [Organic Maps](https://organicmaps.app/)  

**Warnings**:  
- Banking apps need [Shelter](https://github.com/PeterCxy/Shelter) isolation  

---

### 3. 🔥 Pro Tier: "Zero-Trust Mobile"  
*For Google-free life*  

**Threat Model**: Eliminate Google dependencies  
**Tools**:  
- [GrapheneOS](https://grapheneos.org/) (Pixel only)  
- [RethinkDNS](https://github.com/celzero/rethink-app) (Block `clients*.google.com`)  
- [Nextcloud](https://nextcloud.com/) (Self-hosted)  

**Warnings**:  
- No Google Pay/WearOS  
- Camera quality loss  

---

### 4. ☢️ Pro++ Tier: "Fortress Mode"  
*For journalists/activists*  

**Threat Model**: Anti-surveillance/anonymity  
**Tools**:  
- Baseband removal (Wi-Fi only)  
- Tor → VPN → Tor via [Orbot](https://guardianproject.info/apps/org.torproject.android/)  
- [Briar](https://briarproject.org/) (Offline mesh)  

**Warnings**:  
- 40%+ app incompatibility  
- High maintenance  

---

## Core Toolkit  

### Google Alternatives  
| **Service**   | **Replacement**                     |  
|---------------|-------------------------------------|  
| Play Store    | Aurora Store (Sandboxed)            |  
| Chrome        | Vanadium/Mullvad Browser            |  
| Docs          | LibreOffice + Cryptpad              |  
| Maps          | OSMAnd (Offline)                    |  

### Advanced Tools  
- [CanvasBlocker](https://addons.mozilla.org/en-US/firefox/addon/canvasblocker/)  
- [Syncthing](https://syncthing.net/) (Google Drive replacement)  
- [Leta](https://leta.mullvad.net/) (Mullvad's private search)  

---

## Critical Warnings  
1. **Banking Apps**:  
   - Isolate in [Shelter](https://github.com/PeterCxy/Shelter)  
   - Use Aurora Store *anonymous mode*  
2. **Location Tracking**:  
   - Disable Wi-Fi/Bluetooth scanning  
   - Set `captive_portal_https_url` to non-Google endpoint  

---

## Implementation Roadmap  
1. **Week 1**: Light tier (debloat + browser swap)  
2. **Month 1**: Normal tier (CalyxOS + DNS filtering)  
3. **Month 3**: Pro tier (GrapheneOS + self-hosting)  
4. **Ongoing**: Pro++ hardening  

---

**Resources**:  
- [The Hated One's Video](https://youtube.com/watch?v=...)  
- [LINDDUN Framework](https://www.linddun.org/)  
- [GrapheneOS Install Guide](https://grapheneos.org/install)  
