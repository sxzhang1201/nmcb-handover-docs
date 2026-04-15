# Recurring study routines

Mailbox triage, logs, screeners, and ad hoc reporting—tasks that keep the study running but are not a single named “pipeline” like CDL or devices.

## Weekly NMCB mailbox

### Purpose

Monitor the shared mailbox so time-sensitive operational items are not missed.

### Frequency

Weekly at minimum; more often during active recruitment or heavy participant contact.

### Inputs

- access to the shared mailbox  
- current contact list  
- current routing rules or responsibilities  

### Steps

1. Review unread or new messages.  
2. Classify: participant communication; scheduling / visit follow-up; data issue; device issue; researcher request; administrative.  
3. Forward or assign when outside your ownership.  
4. Record actions in the relevant log or tracker.  
5. Flag unresolved items that need follow-up.

### Output

Mailbox triaged; urgent issues routed; actions logged.

### Quality checks

- No urgent participant-facing email left unassigned.  
- Data problems have an owner.  
- Follow-up deadlines visible outside the inbox.

---

## Weekly visit log

### Purpose

Accurate overview of completed, pending, and problematic visits.

### Frequency

Weekly.

### Steps

1. Compare planned vs completed visits.  
2. Update visit date, visit type, status.  
3. Note rescheduling, incomplete procedures, or data issues.  
4. Flag visits with pending downstream actions (upload, device return, etc.).

### Quality checks

- Completed visits appear in the log.  
- Incomplete visits visibly flagged.  
- Data tasks can be derived from the log.

---

## Bi-weekly subject ID log

### Purpose

Keep participant identifiers consistent across operational and analytical systems.

### Frequency

Bi-weekly and whenever new participants are added.

### Steps

1. Identify new participants.  
2. Assign or verify subject ID per agreed convention.  
3. Check duplicates or reuse.  
4. Confirm consistency in dependent systems.  
5. Save the log in the agreed location.

### Quality checks

- No duplicate IDs; no accidental gaps.  
- Mapping consistent across logs, Castor, and device outputs.

---

## Bi-weekly send screeners to Linked2Trial

### Purpose

New participants receive general screeners within the expected window (board note: Laurian provides lists; **48-hour** turnaround after receipt).

### Steps

1. Check for a new participant list.  
2. Validate identifiers and contact fields.  
3. Prepare input file or upload package.  
4. Send or upload per agreed workflow.  
5. Record completion date.  
6. Flag participants that could not be processed.

### Quality checks

- 48-hour target where possible.  
- No duplicate participants.  
- Failed transfers logged.

---

## Get numbers

### Purpose

Summary counts for reports, dashboards, or ad hoc asks (eligibility, recruitment, visit completion).

### Frequency

As requested; may be weekly or monthly for routine reports.

### Systems

- [Scripts and QC](../systems/scripts-and-qc.md)  
- [Snowflake](../systems/snowflake.md)  
- [Castor](../systems/castor.md)  

### Steps

1. Clarify metric and period.  
2. Choose script, query, or export.  
3. Run and validate (e.g. vs previous run).  
4. Deliver in agreed format; document method for reproducibility.

---

## Prepare checklist for data routine

### Purpose

Reduce dependence on memory; standardise recurring work.

### Frequency

Update monthly or when operational steps change.

### Steps

1. List recurring tasks by week, month, and ad hoc trigger.  
2. Add owner, backup, expected duration.  
3. Link each item to documentation.  
4. Version the checklist.
