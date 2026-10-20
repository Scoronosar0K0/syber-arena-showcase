# Engineering case study

## Problem

A gaming center needs staff to understand PC availability, run customer sessions and handle purchases, while owners need reports and administration and players need a coherent club experience. These responsibilities span browser applications, central services and Windows devices.

## Approach

The product combines four role-focused web interfaces with Cloud and Edge services and Windows Agent/Client software. React and TypeScript support the browser experiences; C#/.NET services implement business workflows and persistence; Windows software connects those workflows to gaming PCs.

The user interface communicates operational state through the PC map, session information, wallet views and reporting. These are genuine application screens rather than invented portfolio mockups. All published screenshots use an isolated synthetic environment.

## Decisions and trade-offs

| Decision | Benefit | Cost or remaining challenge |
| --- | --- | --- |
| Keep operational capabilities at the club | Selected work can continue when cloud connectivity is interrupted | Synchronization, reconciliation and restore behavior become major engineering concerns |
| Use distinct interfaces for each role | Tasks and navigation can match staff, owner and player needs | Shared business concepts must remain consistent across applications |
| Combine web UI and Windows integration | Consistent presentation with access to desktop/device capabilities | Browser tests cannot establish service, IPC or kiosk behavior |
| Test at several layers | Business rules and cross-application flows can be evaluated separately | Real devices, databases and failure scenarios still need explicit coverage |

## Honest scope

Sessions, billing, cash/POS, wallets/bookings, reporting and PC-control implementation are present. Some workflows are incomplete or require further hardening. This showcase does not claim production availability, a certified security posture, guaranteed offline recovery, measured uptime or completed deployment at a real customer club.

The AI-assisted workflow is part of the engineering context. Generated code and design work contribute to the project; the portfolio does not attribute every line to manual authorship or equate generated volume with product quality.
