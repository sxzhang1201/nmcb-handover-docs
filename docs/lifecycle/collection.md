# Data collection

This stage covers how data is captured at source: study forms, device outputs, and recruitment screeners. Design decisions from [Design](design.md) are implemented here.

## Main collection sources

| Source | Purpose | System |
|--------|---------|--------|
| Study forms and surveys | Participant data, questionnaires | [Castor EDC](../systems/castor.md) |
| Device outputs | Physiological measurements | [Devices](../systems/devices.md) (Nellcor, Tanita, VU-AMS, Amsterdam Cognitive Scan) |
| Recruitment screeners | Linked2Trial screening flow | Linked2Trial exchange |

## Castor EDC

Castor is the main data capture environment for study forms, survey logic, and participant-related study data.

Key hand-over points:

- **Calculations and logic:** Document variable dependencies, formula definitions, expected outputs, and known edge cases.

- **Reminders for incomplete screeners:** Define the query to identify incomplete cases, export the list, review exclusions, send reminders, and record reminder date and outcome.

- **File uploads:** Document allowed file types, naming conventions, size limits, and where uploaded files are retrieved for QC or processing.

## Devices

Device data is captured during visits. Each device has:

- setup before use
- raw output format
- naming convention
- quality control procedure (see [Cleaning](cleaning.md))
- cleaned output or conversion format

## Linked2Trial

The general screeners should be sent within **48 hours** of receiving the participant list.

## Risks

- Hidden logic in Castor form calculations
- Inconsistent use of identifiers across systems
- Reminder processes that are not reproducible
- Dependence on manual exports without versioning
