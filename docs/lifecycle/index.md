# Data lifecycle overview

NMCB data flows through eight main stages. Understanding this flow helps you know where data comes from, how it is transformed, and where it goes.

## The pipeline

```text
Design  →  Collection  →  Storage  →  Cleaning  →  Modelling  →  Issuing  →  Analysis  →  Publication
```

| Stage | What happens | Where |
|-------|--------------|-------|
| **Design** | Planning before collection | Variable definitions, form structure, identifier scheme |
| **Collection** | Data is captured at source | Castor, devices, Linked2Trial |
| **Storage** | Raw and processed data are stored | File structure, Snowflake, biobank |
| **Cleaning** | Quality control and transformation | Device QC, cleaning scripts |
| **Modelling** | Data is structured for analysis | Snowflake, eligibility logic |
| **Issuing** | Data is shared with requesters | Data requests, multicentre transfers |
| **Analysis** | Statistical and exploratory work | Scripts, notebooks |
| **Publication** | Findings and data are made public | Papers, reports, data repositories |

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

1. [Design](design.md) — Planning, variable definitions, identifier scheme
2. [Collection](collection.md) — Castor, devices, Linked2Trial
3. [Storage](storage.md) — File structure, Snowflake, biobank
4. [Cleaning](cleaning.md) — Device QC, conversion scripts
5. [Modelling](modelling.md) — Snowflake structures, eligibility logic
6. [Issuing](issuing.md) — Data requests, multicentre transfers
7. [Analysis](analysis.md) — Statistical and exploratory work
8. [Publication](publication.md) — Papers, reports, data sharing

For detailed system documentation, see the [Systems reference](../systems/data-architecture.md).
