# Data design

This stage covers planning and design decisions made before data collection begins. Good design reduces downstream problems and makes the pipeline easier to maintain.

## What belongs in design

| Topic | Purpose |
|-------|---------|
| Variable definitions | What will be captured and how |
| Form structure | Castor form layout, branching logic |
| Identifier scheme | Subject ID convention, visit numbering |
| Device selection | Which devices, what measurements |
| Template design | Biobank templates, transfer formats |
| Folder structure | Where raw and processed data will live |

## Design principles

- **Identifiers first:** Define the subject ID and visit ID scheme before collection starts. These must be consistent across all systems.

- **Traceability:** Design forms and exports so that every record can be linked back to participant and visit.

- **Separation of concerns:** Plan for raw data, processed data, scripts, and deliverables to live in distinct locations.

## Links to implementation

Design decisions are implemented in:

- [Collection](collection.md) — Castor forms, device setup
- [Storage](storage.md) — Folder structure, Snowflake schema
- [Biobank](../systems/biobank.md) — Sample and biosample templates

## Hand-over note

Document design decisions and their rationale. When the next person inherits the role, they should understand *why* things are structured as they are, not only *how* to operate the pipeline.
