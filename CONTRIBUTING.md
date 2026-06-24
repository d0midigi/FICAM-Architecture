# Contributing to Active Directory FICAM Integration

Thank you for your interest in improving this repository! We welcome contributions that enhance federal compliance, tighten identity architectures, and expand directory automation utilities.

To maintain engineering consistency and prevent regression in security postures, all contributors are expected to follow these guidelines.

---

## 🛠 Working with the Code

### 1. Branch Strategy
Always create features or configuration changes on an isolated topic branch based off the latest version of the `main` branch:
```bash
git checkout main
git pull origin main
git checkout -b feature/your-feature-name
```

### 2. Code Quality & Format Requirements
* **PowerShell Scripts (`.ps1`, `.psm1`):** Must follow the standard `Verb-Noun` naming convention and include comprehensive comment-based help block definitions (`.SYNOPSIS`, `.DESCRIPTION`, `.PARAMETER`).
* **XML Frameworks / GPOs:** Must format clean indentations without unreferenced namespaces.
* **Testing:** All automation logic must pass clean compilation testing in an isolated local Sandbox or Active Directory test environment before submittal.

---

## 🚀 The Pull Request (PR) Process
1. **Verify Documentation:** Ensure any change altering directory architectures includes updates to the localized `/docs/` guides or the core `index.html` file.
2. **Submit PR:** Issue a pull request against the `main` repository branch.
3. **PR Template Checklist:** In your pull request description, please outline the following:
	* **What change was made?** (e.g., Added FIDO2 authentication GPO parameter).
	* **What NIST control does it map to?** (e.g., IA-2, IA-8).
	* **How was it tested?** (e.g., Validated via Windows Server 2022 functional environment).
4. **Code Review:** At least one authorized repository maintainer must review and approve the configuration modifications prior to final merge execution.

--

##❓ Questions or System Issues?
If you identify an architectural gap or security flaw within the configurations, please open an **Issue ticket** on GitHub with complete details highlighting the specific regulatory friction or execution error.
