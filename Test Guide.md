# Ultimate Android Privacy Guide: From Basic to Extreme Measures 
*A Tiered, Evidence-Based Approach to Digital Sovereignty*  


## 🌟 **Two Paths to Freedom**  
Choose your approach based on technical comfort:  
1. **Custom ROM Route**:  
   - Recommended: **Pixel + [GrapheneOS](https://grapheneos.org/)**  
   - Benefit: Full Google removal + security patches  
   - Trade-off: Device-specific support (check [XDA Forums](https://forum.xda-developers.com/))  

2. **Stock ROM Route**:  
   - Debloat + replace apps → Follow this guide  

---

## 🔥 **Core Privacy Workflow**  

---

### **1. Remove/Disable Bloatware**  
**Essential Tool**: [Android Debloat List](https://muntashirakon.github.io/android-debloat-list/print.html)  
*(Trigger print view → Close dialog for full list)*  

**Key Targets**:  
- All Google apps (`com.google.android.*`)  
- OEM bloat (Samsung "Galaxy", Xiaomi "Mi", etc)  
- Carrier apps (Verizon "MyAccount", T-Mobile "Name ID")  

**Safety Protocol**:  
- ❌ **Never Remove**: Critical packages like `com.android.phone`  
- ✅ **Safer**: Use `adb shell pm disable-user` instead of uninstall  

---

### **2. Replace Every Google/OEM App**  
**Often Overlooked Replacements**:  
| System App | FOSS Alternative |  
|------------|------------------|  
| Keyboard | [HeliBoard](https://github.com/Helium314/HeliBoard) |  
| SMS | [QKSMS](https://github.com/moezbhatti/qksms) |  
| Camera | [OpenCamera](https://opencamera.org.uk/) |  
| Gallery | [Fossify Gallery](https://github.com/FossifyOrg/Gallery) |  

**Social Media Workaround**:  
- Instagram → [MyInsta](https://myinsta.app/) (disable Analytics, Ads, and some requests.)  
- YouTube → [Pipepipe](https://github.com/InfinityLoop1308/PipePipe)  

---

### **3. Lock Down Network Access**  
**Essential Tools**:  
| App | Function | Guide |  
|-----|----------|-------|  
| [NetGuard](https://github.com/M66B/NetGuard) | Firewall (no root) | [Blocklist Setup](https://github.com/M66B/NetGuard/blob/master/ADBLOCK.md) |  
| [RethinkDNS](https://github.com/celzero/rethink-app) | DNS Firewall | [OISD Config](https://blitz-setup.rethinkdns.com/oisd) |  

**Advanced Setup**:  
- VPN + Tor via [Orbot](https://guardianproject.info/apps/org.torproject.android/)  
- Always-on VPN: Mullvad/ProtonVPN  

---

### **4. Permission Purge**  
**System-Level**:  
1. *Settings → Apps → [App Name] → Permissions*  
   - Revoke location, microphone, contacts  
2. Use [Bouncer](https://f-droid.org/packages/com.samruston.permission) for temporary access  

**App-Level Enforcement**:  
```bash 
# Restrict background internet (ADB)
adb shell cmd appops set <package> RUN_IN_BACKGROUND ignore
```

---

### **5. Account & Tracking Prevention**  
**Golden Rules**:  
- Never use "Sign in with Google"  
- Use unique emails via [SimpleLogin](https://f-droid.org/packages/io.simplelogin.android.fdroid/)  
- Disable:  
  - *Settings → Location → Wi-Fi/Bluetooth scanning*  
  - *Settings → Security → Device admin apps*  

---

## 🛠️ **Privacy Toolkit**  

---

### **App Stores**  
| Purpose | Tool |  
|---------|------|  
| Main Store | [Neo Store](https://github.com/NeoApplications/Neo-Store/) (F-Droid client) |  
| Play Alternative | [Aurora Store](https://gitlab.com/AuroraOSS/AuroraStore) (anonymous mode) |  
| Direct Updates | [Obtainium](https://github.com/ImranR98/Obtainium) (GitHub/GitLab) |  

---

### **Browser Setup**  
1. Install [Firefox](https://www.mozilla.org/firefox/mobile/)  
2. Addons:  
   - [uBlock Origin](https://addons.mozilla.org/firefox/addon/ublock-origin/)  
   - [ClearURLs](https://addons.mozilla.org/firefox/addon/clearurls/)  
   - [LocalCDN](https://addons.mozilla.org/firefox/addon/localcdn-fork-of-decentraleyes/)  
3. Settings:  
   - `about:config → privacy.resistFingerprinting = true`  

---

### **Health/Activity Privacy**  
1. Disable:  
   - Google Fit/Samsung Health  
   - Step counters in system settings  
2. Alternatives:  
   - [OpenTracks](https://github.com/OpenTracksApp/OpenTracks) (GPS logging)  
   - [Health Connect](https://play.google.com/store/apps/details?id=android.healthconnect.console) (local storage)  

---

## ☢️ **Extreme Measures**  

---

### **Physical Mods**  
1. **Baseband Removal**:  
   - Disable cellular modem via hardware mod (advanced users only)  
2. **Wi-Fi Only Mode**:  
   - Remove SIM card + *Settings → Network → Airplane mode*  

---

### **Communication Lockdown**  
| Purpose | Tool |  
|---------|------|  
| Calls/SMS | [Silence](https://silence.im/) (encrypted SMS) |  
| Email | [ProtonMail](https://proton.me/mail) + [PGP](https://openkeychain.org/) |  
| Chat | [Briar](https://briarproject.org/) (offline mesh) |  

---

## 🔄 **Maintenance Routine**  
1. Monthly:  
   - Audit app permissions  
   - Check [F-Droid Updates](https://f-droid.org/updates/)  
2. Quarterly:  
   - Review firewall rules  
   - Test backup restoration  

---

**"Privacy Isn't All-or-Nothing"** - Start with Light tier, escalate as needed. Even basic steps (disable Google apps + use NetGuard) significantly reduce tracking!

**Full Resource List**:  
- [Privacy Guides](https://www.privacyguides.org/)  
- [FOSS Android Apps](https://github.com/offa/android-foss)  
