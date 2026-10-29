# Judo Ceremony Desk 0.13 — portable event backup

Version 0.13 includes the event readiness panel and reviewed IJF medal-result import from 0.12, plus a portable backup for moving an event to another PC.

## Create a backup

Select **Event backup…** at the top of the desk, then **Create backup ZIP…**. Choose a destination such as a local folder or USB drive. The app creates a `.judo-backup.zip` without uploading anything or modifying the current preparation.

The ZIP includes the event name, settings, categories, saved medal countries and layouts, country filters, imported event details, independent output preferences, hashtag, embedded background and logos. It also includes imported MP3/WAV recordings for the event's participating or medal countries. Other event history and unrelated recordings are excluded. Bundled flags and recordings come with the installed application and are not duplicated into the backup.

The manifest records the size and SHA-256 of the event and each included recording. Keep the ZIP private if the event information or imported recordings are private. A backup contains data, not the Windows application itself.

## Restore on another PC

1. Install or extract Judo Ceremony Desk **0.13 or newer** on the other Windows PC.
2. Select **Event backup… → Restore backup → Choose backup ZIP…**.
3. Review the event, saved-category count and included recordings.
4. Leave **Replace matching local recordings with backup versions** unchecked to keep existing local overrides. Identical recordings are kept automatically. If replacement is selected, it changes the shared recording for that country across events on that PC; stop the anthem and reset an active flag rise first.
5. Select **Restore as new event**. The app saves a new event identity and retains previous event history. Preparation starts empty; select a category to restore its saved countries.

The loaded audience ceremony and its playing anthem are retained. Restoring new files or keeping existing overrides does not automatically load the restored event to the audience. Explicit replacement of a stopped shared recording can update the selected recording; playing/paused audio and active/paused flags prevent that replacement.

The restore preview lists recordings as new, identical or conflicting. It checks all payload hashes, event structure, embedded artwork, country mappings and audio headers before applying anything. Damaged, unsupported or unsafe ZIPs are rejected. Closing the preview does not restore it. Imported recordings still need playback and venue checks; a valid audio header alone does not certify the recording version or Windows decoding.

## Limits and recovery

Backups and expanded content are limited to **2 GB**, event JSON to **25 MB**, and each recording to **100 MB**. Up to 255 imported country recordings are supported. The ZIP accepts only the declared event and audio entries; paths outside its expected structure, duplicate entries and symbolic links are rejected.

An interrupted or failed export keeps any existing destination ZIP. A normal restore failure rolls back recording changes, the previous session and history index, and removes its partial new event. The source backup ZIP is never modified. If an external disk/permission problem also prevents rollback, the error identifies retained recovery copies rather than deleting them.

Backups use **backup format 1** with an embedded **schema 5** event. Event JSON files remain compatible with 0.11/0.12; restoring the portable ZIP requires 0.13 or newer. Ordinary Open/Save tournament files remain available and do not contain audio files.

## Validation

Checks cover an isolated second-PC setup, multiple category results, embedded branding, event-specific audio selection, local recording conflicts, new event identity, rollback after simulated audio/session failures, staging tampering, corrupt/missing/future/unsafe ZIP entries, cancelled export, UI preview/cancel, and preservation of the loaded audience ceremony and anthem. Readiness, IJF imports and all previous checks are retained.

**432 software checks passed**, including native Windows decoding of all 146 bundled recordings, backup rollback, UI restore and all earlier readiness/results checks. Package verification also checks native launch, fresh startup, icon and all 442 reference-image hashes.
