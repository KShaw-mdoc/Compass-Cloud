# Certiport Compass Cloud – Resident EDU Network

This repository provides **approved Certiport Compass Cloud installers** for devices used across the Resident Education (Res EDU) network.

Installers are distributed exclusively via **GitHub Releases** to ensure:

- ✅ Controlled version management  
- ✅ Rollback capability  
- ✅ Consistent deployment across facilities  
- ✅ Stable direct URLs for scripting, MDM, and RMM systems  
- ✅ Clean separation between documentation (main branch) and production binaries (Releases)  

---

## 📦 Repository Structure

### Main Branch
- Documentation only (`README.md`)
- No installer binaries stored in source control

### Releases
- Version-tagged installers
- Windows `.msi`
- macOS `.dmg`
- Immutable historical versions retained for rollback

This structure ensures traceable version history and production-grade hygiene.

---

## 🏷️ Current Approved Release

| Version | Windows (.msi) | macOS (.dmg) |
|----------|----------------|--------------|
| **v2026.1** | [Download MSI](https://github.com/KShaw-mdoc/Compass-Cloud/releases/download/v2026.1/CompassCloudSetupProd.msi) | [Download DMG](https://github.com/KShaw-mdoc/Compass-Cloud/releases/download/v2026.1/CompassCloud.dmg) |

🔗 Browse all releases:  
https://github.com/KShaw-mdoc/Compass-Cloud/releases

---

## 🔗 Direct Download URLs (Automation Use)

### v2026.1

**Windows (.msi)**  
https://github.com/KShaw-mdoc/Compass-Cloud/releases/download/v2026.1/CompassCloudSetupProd.msi  

**macOS (.dmg)**  
https://github.com/KShaw-mdoc/Compass-Cloud/releases/download/v2026.1/CompassCloud.dmg  

---

# 🚀 Deployment Guidance

## 💻 Windows Deployment

1. Download the `.msi` from the approved release.
2. Install manually or deploy through RMM/automation.

### Silent Install (Standard)

```bat
msiexec /i CompassCloudSetupProd.msi /qn
