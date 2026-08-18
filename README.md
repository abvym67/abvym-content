# abvym-content

Content for the ABVYM Unit Guide Android application, published by
Akhil Bharat Vivekananda Yuva Mahamandal.

`abvym_entries_v1.json` holds the whole question-and-answer library in English,
Bengali and Hindi. Every installed copy of the app checks this file on launch,
and downloads it only when its `version` number is **higher** than the one the
phone already holds.

## Before editing, read this

- **Never rename, move or delete `abvym_entries_v1.json`.** Its address is
  compiled into every copy of the app already on a phone:
  https://raw.githubusercontent.com/abvym67/abvym-content/main/abvym_entries_v1.json
- To publish a correction: edit the file, raise the `version` number
  (for example 1.8 to 1.9), and commit to `main`. Phones take it up within
  minutes, on their next launch.
- **Never raise the version number of a file that is behind the app's own
  bundled copy.** That would push older content over newer. If in doubt,
  compare with `app/src/main/assets/abvym_entries_v1.json` in the app project.
- Editing without raising the number is safe: nothing travels until it rises.
- Commit to `main`. Work on a branch reaches no phone until it is merged.

All rights reserved.
