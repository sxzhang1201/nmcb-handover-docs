# Multi-centre sample data workflow

## Multi-centre sample processing

1. After blood tubes are drawn, **research nurses** open `Data lab NMCB  - Blood tubes file.xlsm`, use the 2nd column **`lab_sample_id`**, scan barcodes of all blood tubes, and add **Participant ID** in the 1st column **`participant_ID`**. Rename the file to `Data lab NMCB  - Blood tubes file.xlsm - {participant_id}` and send it to the lab that processes samples at the Radboud site.
2. The Radboud lab (**RL**) completes the remainder of the file (e.g. `datetime_collection`, `start_datetime_processing`, `finish_datetime_processing`, `datetime_freezer`, `aliquot_nr`, …). Upload the raw **RL** file to the agreed location on Research Drive.
3. **Data team** processes the raw RL file with the agreed Python pipeline. Move the raw file to `organized/RL/archive` and upload the output to `processed/RL/` as `processed_{participant_ID}_RL.csv`.

**To improve:** (1) guidance on how to fill in the `.xlsm` (2) SOP for uploading.

---

## Sample boxing

1. When a sample box is full and delivered to Amsterdam UMC biobank, upload the **Box Data File** to NMCB Research Drive. Each box needs a unique ID and naming per **SOP: how to rename box data file**.
2. **Data team** expands the Box Data File by adding columns from existing RL files—linking each sample row to the source participant and processing metadata. The result is the **Biobank Submission File**.
3. Another **data team** member validates (spot-check or scripts). Send the validated file to the biobank via FileSender. Current contacts: Erik and Maureen.

**To improve:** (1) SOP on **how to rename box data file** (2) SOP on uploading.

## Related

- [Sample request workflow](sample-request-workflow.md)
- [Systems: Biobank](../systems/biobank.md) — short system pointer
