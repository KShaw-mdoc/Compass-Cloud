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

```
msiexec /i CompassCloudSetupProd.msi /qn
```

Confirm Before Test Day

Administrative rights available (if required)

Firewall and network access validated

Version matches Certiport requirements

Successful test launch under student account

🍎 macOS Deployment

Download the .dmg from the approved release.

Mount the DMG.

Install per Certiport guidance.

MDM Deployment (Mosyle or Similar)

Upload DMG or converted PKG as required

Assign to correct Smart Group

Validate installation on a pilot device

Confirm successful application launch

🧪 Pre-Test Validation Checklist

Before scheduling exams:

Confirm Compass Cloud version alignment with Certiport guidance

Validate outbound network/firewall rules

Confirm camera/microphone permissions (if required)

Verify correct local user permissions

Test login and exam launch on at least one lab device

Validate automated/silent deployment behavior

🔐 Compliance & Scope

This repository contains installer files only.

No exam content, credentials, licensing keys, or student data are stored here.

Distribution and usage must comply with Certiport vendor policy.

Only validated versions should be used in production environments.

🔄 Version Governance

Version tags follow format: vYYYY.X

Prior releases remain available for rollback

Only approved versions are designated as Latest

New releases should be validated prior to lab-wide deployment

📞 Support & Version Approval

For Compass Cloud deployment support or version approval:

📧 Kenneth.Shaw@maine.gov
