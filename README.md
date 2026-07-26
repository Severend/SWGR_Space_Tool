# SWGR ROGUE Space Tool

A single-file, browser-based planning tool for **Star Wars Galaxies: Restoration**
ROGUE-era ship components and loadouts. Open `SWGR-ROGUE-Space-Tool.html` in any
modern browser — no install, no server, everything runs locally.

## Files

| File | What it is |
| --- | --- |
| `SWGR-ROGUE-Space-Tool.html` | The tool. Download and open it in a browser. |
| `community-sync.csv` | Community pool of **observed** component rolls, used by the tool's sync feature. |

## The community sync file

`community-sync.csv` is a shared, curated dataset of component stat rolls that
players have observed on the server. It lets the tool show realistic stat ranges
without every player having to catalogue components from scratch.

- Every row is marked `Observed` — it is reference data, not anyone's inventory.
- It contains **no personal ship loadouts and no `Owned` parts**.
- Parts are identified by their **stats**, so blank or partial names are fine.

## Contributing data

Data is curated manually to keep the shared file clean and to prevent bad rolls
from propagating:

1. In the tool, export your observed components.
2. Send the export to the maintainer.
3. The maintainer reviews the diff and merges it into `community-sync.csv`.

Because the file lives in Git, every change is versioned and any bad merge can be
rolled back.
