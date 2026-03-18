# Data storage

This stage covers where data is stored: file structures, Snowflake, and biobank systems.

## Storage locations

| Location | Purpose | System |
|----------|---------|--------|
| Research drive | File storage, raw and processed data | File structure |
| Snowflake | Structured data, analytical queries | [Snowflake](../systems/snowflake.md) |
| Biobank | Sample metadata, biosample data | [Biobank](../systems/biobank.md) |

## Folder design principle

A good storage structure should separate:

- raw data
- processed data
- scripts
- logs
- documentation
- outgoing deliverables

## File structure

See [Where everything lives](../where-everything-lives.md) for the current map of folders, owners, and permissions.

Key locations include:

- Device raw data (organised by device and date)
- Device QC outputs (versioned folders preferred)
- Scripts (prefer Git version control)
- Snowflake / SQL setup

## Snowflake

Snowflake is used for:

- structuring study data more systematically
- reducing manual transformations
- supporting downstream extraction and reporting

Document access model, connection details, and key tables or views.

## Biobank

Biobank storage includes:

- sample metadata
- fecal sample data template
- biosample data template (except fecal sample)

Template governance is critical: define which template is current, version, owner, and mandatory columns.
