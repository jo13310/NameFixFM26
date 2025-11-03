# FM26 Open Names Pack

Community-maintained Football Manager 2026 real names data merged into a single, comment-free `.lnc` file. The dataset condenses popular public fixes, deduplicates overlapping entries, and sorts everything for easier peer review. The goal is to provide an open, source-agnostic foundation that anyone can extend.

## Features
- One canonical `FM26-open-names.lnc` covering competitions, clubs, people, stadiums, and awards.
- All comments, credits, and duplicate rules removed for a neutral, clean baseline.
- Alphabetically sorted entries so diffs reveal meaningful gameplay changes.
- Packaged for FM Reloaded Mod Manager with manifest, changelog, and CC0 licence.

## Installation

### Using FM Reloaded Mod Manager
1. Place this repository in your FM Reloaded `mods` workspace.
2. Launch FM Reloaded and install **FM26 Open Names Pack**.
3. FM Reloaded copies `FM26-open-names.lnc` into `shared/data/database/db/2600/lnc/all/`.
4. Apply the **Manual cleanup** steps below so legacy licensing files do not undo the changes.
5. Restart Football Manager 26. Existing saves update immediately (Brazilian clubs still require a new save).

### Manual install (zip download)
1. Download the latest release archive and extract it.
2. Copy `assets/lnc/FM26-open-names.lnc` into `Football Manager 26/shared/data/database/db/2600/lnc/all/`.
3. Continue with the manual cleanup steps below.

### Manual cleanup (recommended)
Remove the stock licensing artefacts so the open names file takes effect everywhere:

- From `shared/data/database/db/2600/lnc/all/` delete:
  - `ac milan (wom).lnc`
  - `acc Inter unlic 26.lnc`
  - `acmilan unlic 26.lnc`
  - `fake.lnc`
  - `inter (wom).lnc`
  - `inter unlic 26.lnc`
  - `japanese names.lnc`
  - `lazio (wom).lnc`
  - `lic_dan_swe_fra.lnc`
  - `licensing club name_fm26.lnc`
  - `men lazio.lnc`
  - `men.atalanta.lnc`

- From `shared/data/database/db/2600/edt/permanent/` delete:
  - `fake.edt`

- From `shared/data/database/db/2600/dbc/permanent/` delete:
  - `1_japan_removed_clubs.dbc`
  - `brazil_kits.dbc`
  - `england.dbc`
  - `forbidden names.dbc`
  - `france.dbc`
  - `japan_fake.dbc`
  - `japan_unlicensed_random_names.dbc`
  - `j league non player.dbc`
  - `licensing_post_data_lock.dbc`
  - `licensing2.dbc`
  - `licensing26.dbc`
  - `netherlands.dbc`

- From `shared/data/database/db/2600/dbc/language/` delete:
  - `Licensing2.dbc`
  - `Licensing2_chn.dbc`

### Updating
- **Existing saves**: Everything except Brazilian clubs updates instantly; start a new save to refresh those.
- **New database drops**: When Sports Interactive ships an updated database (e.g., `2640`), copy `FM26-open-names.lnc` into the new `lnc/all/` folder and repeat the cleanup routine.
- **Contributions**: Submit pull requests or share diffs that adjust the single `.lnc` file; keep entries sorted.

## Licence
Released under [CC0 1.0 Universal](LICENSE). Use it, remix it, and redistribute it without attribution requirements.
