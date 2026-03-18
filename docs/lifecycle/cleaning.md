# Data cleaning

This stage covers quality control and transformation of raw data before it is used for analysis.

## Main cleaning activities

| Activity | Purpose | System |
|----------|---------|--------|
| Device QC | Validate and clean device outputs | [Devices](../systems/devices.md) |
| Conversion scripts | Standardise formats (Omron, Tanita, Nellcor, M&L) | [Scripts](../systems/scripts.md) |
| Python/R cleaning | Clean raw data, quality control | [Scripts](../systems/scripts.md) |

## Device QC

For each device, document:

1. setup before use
2. raw output format
3. naming convention
4. quality control procedure
5. cleaned output or conversion format

### Device-specific notes

- **Nellcor:** Date format change from MM/DD/YY to DD/MM/YY — device settings matter for downstream matching.

- **Tanita:** Difference between onsite Tanita Pro and portable home-visit Tanita data; document field mappings and how outputs are standardised.

- **VU-AMS:** Document expected file pattern, abnormal export patterns, QC script or manual process, and pass/fail criteria.

- **Amsterdam Cognitive Scan:** Document QC checks, completeness criteria, and how output links to participant ID.

## Scripts

Scripts for cleaning and conversion should be documented with:

- repository or folder location
- language and package dependencies
- how to run
- required inputs
- produced outputs
- validation or QC rule

## Automation opportunities

The board suggests repeated interest in reducing manual work around:

- raw file cleaning and QC
- standardising conversion code

These are strong candidates for future formal pipelines rather than person-dependent scripts.
