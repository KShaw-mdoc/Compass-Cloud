# Certiport Compass Cloud – Resident EDU Network

This repository contains approved **Certiport Compass Cloud** installers for devices used across the Resident Education (Res EDU) network.

The installers are version-controlled and distributed via GitHub Releases to ensure consistent deployment across facilities.

Designed for:

✅ Windows lab deployment (manual or scripted)  
✅ macOS deployment (manual or MDM-based)  
📦 Centralized version control  

---

# 📦 Contents

This repo includes:

• `.msi` files for Windows (silent install support)  
• `.dmg` files for macOS  
• Releases organized by version tag  

---

# 🏷️ Releases by Version

Click to download the Windows and macOS installers for each version:

| Version | Windows (.msi) | macOS (.dmg) |
|----------|----------------|--------------|
| v2026.1 | Download | Download |
| v2026.2 | Download | Download |

🔗 Browse all releases:  
https://github.com/KShaw-mdoc/Certiport-CompassCloud/releases

---

# 🔗 Direct URLs (for scripting or documentation)

After publishing a release, the download URLs will follow this structure:

### v2026.1 Example

| Platform | Direct URL |
|----------|------------|
| Windows | https://github.com/KShaw-mdoc/Certiport-CompassCloud/releases/download/v2026.1/compass_cloud_windows_v2026.1.msi |
| macOS | https://github.com/KShaw-mdoc/Certiport-CompassCloud/releases/download/v2026.1/compass_cloud_macos_v2026.1.dmg |

---

# 🚀 Deployment Instructions

## 💻 Windows Deployment

1. Download the appropriate `.msi` from the Releases page.
2. Install manually or deploy via RMM/script.

Silent install example:


msiexec /i compass_cloud_windows_v2026.1.msi /qn


You may add additional MSI parameters if required by Certiport documentation.

---

## 🍎 macOS Deployment

1. Download the `.dmg` from the Releases page.
2. Mount the DMG.
3. Install according to vendor instructions.

If deploying through Mosyle or another MDM:
• Upload the DMG or converted PKG as required  
• Assign to appropriate Smart Group  
• Confirm installation prior to test day  

---

# 🧪 Pre-Test Validation Checklist

Before scheduling Certiport exams:

• Confirm Compass Cloud version matches Certiport requirements  
• Verify network/firewall access  
• Confirm camera/microphone permissions (if required)  
• Ensure local user permissions are correct  
• Test launch on at least one device per lab  

---

# 🔐 Notes

• This repository contains installers only.  
• No exam content, credentials, or licensing data are stored here.  
• Ensure compliance with Certiport distribution policies.  

---

# 📞 Contact

For Certiport / Compass Cloud deployment support or version management:

📧 Kenneth.Shaw@maine.gov
