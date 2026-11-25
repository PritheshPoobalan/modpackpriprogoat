# Project structure

This document describes the recommended layout of the modpack repository.

## Directories

| Directory | Purpose |
|-----------|---------|
| `docs/` | Project documentation such as usage and structure guides. |
| `example/` | Example files, including a sample modpack manifest. |
| `mods/` | Mod archives included in the modpack (not tracked by default). |
| `overrides/` | Optional files that override default game resources (configs, scripts). |

## Key files

| File | Purpose |
|------|---------|
| `README.md` | Project overview, getting started, and contributing instructions. |
| `docs/usage.md` | Step-by-step usage guide. |
| `docs/project-structure.md` | This document. |
| `example/sample-modpack.json` | Example modpack manifest. |
| `.gitignore` | Files and directories excluded from version control. |
| `LICENSE` | License under which the project is released. |

## Manifest format

The sample manifest in `example/sample-modpack.json` uses this shape:

```json
{
  "modpack": {
    "name": "Example Modpack",
    "version": "1.0.0",
    "game_version": "1.20.1",
    "loader": "forge",
    "loader_version": "47.2.0"
  },
  "mods": [
    {
      "name": "Example Mod",
      "file": "example-mod.jar",
      "version": "1.0.0",
      "url": "https://example.com/mods/example-mod"
    }
  ]
}
```

Keep the manifest in sync with the contents of `mods/`: every file listed must
exist, and every file in `mods/` should be listed.
