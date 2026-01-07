# PHTI Contract Tool Data

This repository contains JSON files that populate the PHTI Contract Tool forms.

The PHTI Contract Tool plugin reads these files directly from GitHub via API at runtime.

The purpose of this separation is so that content updates are quick and easy and do not need to involve Alley. Additionally, version control is automatic through GitHub. When these files change in the `main` branch, the forms will automatically show the updated content.
