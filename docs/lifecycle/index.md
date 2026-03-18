# Data lifecycle overview

NMCB data flows through five main stages. Understanding this flow helps you know where data comes from, how it is transformed, and where it goes.

## The pipeline

```text
Collection  →  Storage  →  Cleaning  →  Modelling  →  Distribution
```

| Stage | What happens | Where |
|-------|--------------|-------|
| **Collection** | Data is captured at source | Castor, devices, Linked2Trial |
| **Storage** | Raw and processed data are stored | File structure, Snowflake, biobank |
| **Cleaning** | Quality control and transformation | Device QC, cleaning scripts |
| **Modelling** | Data is structured for analysis | Snowflake, eligibility logic |
| **Distribution** | Data is shared with requesters | Data requests, multicentre transfers |

## Core principle

**Identifiers and provenance must survive every transformation step.**

Every workflow should make it possible to answer:

- Where did this record originate?
- Which script or process changed it?
- Which identifier links it back to the participant or visit?
- Is the current dataset raw, intermediate, or analysis-ready?

## Current infrastructure status

The task board shows active work on:

- building a diagram of the data pipeline
- designing file structures in the research drive
- testing SQL setup and Snowflake connectivity
- standardising conversion code for device-derived data
- improving extraction flow by combining patient-centric and source-centric approaches
- exploring automated eligibility logic in Snowflake
- mapping NMCB data toward OMOP

This suggests the infrastructure is still evolving and should be documented as a living system rather than a finished platform.

## Next steps

Use the lifecycle pages to understand each stage:

1. [Collection](collection.md) — Castor, devices, Linked2Trial
2. [Storage](storage.md) — File structure, Snowflake, biobank
3. [Cleaning](cleaning.md) — Device QC, conversion scripts
4. [Modelling](modelling.md) — Snowflake structures, eligibility logic
5. [Distribution](distribution.md) — Data requests, multicentre transfers

For detailed system documentation, see the [Systems reference](../systems/data-architecture.md).
