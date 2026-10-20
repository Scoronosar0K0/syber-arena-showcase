# Verification scope

Prepared from a private implementation review on 20 October 2026. A review of source and test files establishes what exists; it does not establish that every test currently passes.

| Evidence | What it supports | Limit |
| --- | --- | --- |
| Service/domain test projects | Automated checks exist for application behavior | No new complete .NET run was executed for this showcase preparation |
| PostgreSQL integration test sources | Database-bound behavior has dedicated test code | Current database integration status was not rerun here |
| Vitest and Playwright sources | Component and browser workflow verification is part of the project | No new complete web suite run was executed for this preparation |
| Genuine local UI captures | Selected screens operate with synthetic demonstration data | Captures do not establish production use or every visible feature |
| Windows-specific procedures | Device behavior is treated as a separate concern | No new real-device, kiosk-escape or installation validation is claimed |

Historical test totals are intentionally omitted because this showcase preparation did not reproduce them. Known open work includes operational hardening and more complete failure/recovery validation. No quantified security, reliability or performance claim is made.

The original implementation and its history remain private. This repository was initialized independently with selected showcase materials, rather than inheriting the production Git history.
