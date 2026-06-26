# PHTI Contract Tool Data

This repository contains JSON files that populate the PHTI Contract Tool forms.

The PHTI Contract Tool plugin reads these files directly from GitHub via API at runtime.

The purpose of this separation is so that content updates are quick and easy and do not need to involve Alley. Additionally, version control is automatic through GitHub.

- `main` is connected to PHTI's production site (https://phti.org)
- `staging` is connect to our staging site (https://dev-phti.pantheonsite.io/)

The https://github.com/alleyinteractive/phti-contract-tool repository contains the functionality for the PHTI contract tool. In that repository, there is functionality that fetches these files using the `/form-config/` endpoint. By default, it will fetch directly from GitHub, but you can override the source via the `phti_contract_tool_data_url` option, e.g. `wp option set phti_contract_tool_data_url https://raw.githubusercontent.com/alleyinteractive/phti-contract-tool-data/staging`
