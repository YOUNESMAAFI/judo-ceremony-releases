# Judo Ceremony Desk 0.10 — offline anthem playback

This local preview adds audio to **2 Ceremony display**. Staff images and tournament file schema 4 are unchanged. The public 0.9 release does not contain audio; use the 0.10 application for the controls below.

## Separate controls first

Loading a ceremony selects its gold winner's three-letter country code and opens the local recording without playing it. A ceremony with no gold selects no anthem. Choose a country manually when needed. Changing preparation, selecting another category, opening history or switching tabs does not replace the loaded anthem.

The anthem has its own **Play / Pause / Stop / Restart**, progress, duration and volume. **Play** resumes paused music; after it finishes, Play starts it again. **Stop** returns the music to its beginning. Music can run before the flags, after the flags, or with no audience window when controls are separate. Flags remain at their final height when music ends. Closing the application closes its audio decoder and stops music.

**Test sound** plays a two-second tone through the Windows default audio output. Choose the venue speakers in Windows sound settings and test the connection before playing a recording. The tone is separate from the selected anthem and never raises flags. Changing the recording is disabled while an anthem is playing or paused; Stop first.

## Optional linking

**Link anthem and flag controls** starts unchecked each time the app opens. Checking it never starts playback. Choose the link setting before starting; it is locked while either output is active.

When linked, the Play, Pause and Restart buttons in either panel operate both outputs. **Stop / Reset** stops the anthem and returns flags to their starting positions, with confirmation while a ceremony is active. Existing flag shortcuts also operate linked audio. Black screen pauses linked audio; restoring the picture does not resume it automatically. Closing or disconnecting the audience display pauses linked music. With separate controls, flag operations do not change the music.

Both the loaded ceremony and a ready recording are required before linked playback can start. Missing, loading or failed audio cannot silently start the flags. A decoder failure pauses a linked flag rise. If the flags finish first, the music continues and can still be paused and resumed with the linked controls. If music finishes first, the flags finish their configured rise. Restart begins both again.

## Recordings and imports

The bundled library contains 146 selected instrumental U.S. Navy Band performances documented by their original Wikimedia Commons file pages. Recordings come from Commons originals/derivatives, source-matched public-domain mirrors and an archived original Navy source for USA. `Assets/Anthems/catalog.json` records each recording's country code, original page, performer, license metadata, acquisition source and SHA-256. The mapping is explicit; historical and questionable entries are not assigned merely by guessing a filename. These are reference recordings, not a claim of IJF approval or of the version required by a particular event. Rehearse the recording selected for each winning country.

**Import file…** copies a preferred recording for the selected country into `%LOCALAPPDATA%\JudoCeremony\anthems`, using a filename such as `TJK - Tajikistan.mp3`. Local imports override bundled recordings. **Use bundled** removes that country's imported override and returns to the supplied track, where available. Your source file is not changed.

**Import folder…** reads MP3/WAV files directly in a chosen folder whose names begin with a known three-letter code, such as `FRA.mp3`, `TJK - Tajikistan.wav` or `GER_Anthem.mp3`. It rejects duplicate recordings for one code before importing. Unrecognised filenames are skipped and counted. Imported files must have a matching audio header and be at most 100 MB; Windows checks decoding when opening a track. Files that cannot play are shown as failed, with replacement available.

Recordings are shared on this PC across events. The link checkbox, selected manual anthem and volume are session controls. Audio files are not embedded in tournament exports or event-history files. To move your overrides to another PC, copy the `anthems` folder into that PC's Judo Ceremony data directory. A `--data-dir` rehearsal has its own imported library.

The application makes no network requests for playback. A country outside the included library shows **No recording available** and supports importing a preferred version. Coverage and source review are documented in `ANTHEM-LIBRARY.md`.

## Anthem testing panel

Open **4 Anthem testing** to browse all 255 country/delegation entries independently of the loaded ceremony. Search by three-letter code or country name, then filter **All countries**, **Available**, **Missing** or **Needs attention**. The table distinguishes bundled recordings from local imports. Failed recordings are marked Needs attention when tested; Refresh reloads current file availability.

Select a row to see its flag and load the recording without autoplay. Use the panel's own **Play / Resume, Pause, Stop and Restart**, seek slider, elapsed time and volume to listen to any part of the track. **Refresh** discovers newly imported or replaced files. Missing recordings can be imported on Ceremony display and then refreshed here.

The test player does not change medal countries, flag positions, the selected ceremony anthem, link preferences or the ceremony volume. Test audio stops when leaving this tab or starting ceremony playback. Listening is blocked while ceremony audio is playing or paused, or while a flag rise is running or paused. Browsing remains available. Space operates the focused preview control; the function keys remain ceremony shortcuts.

## Validation

Checks cover separate and linked transport, both end orders, pause/resume after flags finish, missing and loading recordings, decoder failure, blackout, display disconnect, no-gold selection, local import/restore, file hashes, native MP3/WAV opening and the actual operator controls. Additional tests cover country filtering, test playback and seeking, tab changes, overlapping-audio prevention, missing/corrupt previews and minimum-size layout. Native playback checks use zero volume and isolated data. The actual venue speakers and HDMI connection still need an audible rehearsal.
