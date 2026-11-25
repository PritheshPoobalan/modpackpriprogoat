# Usage guide

This document explains how to assemble and use the modpackpriprogoat modpack
after installation.

## Step 1: Choose a loader

Pick a mod loader that matches the game version you target. Common choices are
Forge, Fabric, and Neoforge. The loader must be installed before any mods can
run.

## Step 2: Add mods

Place mod files (typically .jar or .zip archives) in the mods/ directory.
For each mod, add an entry to example/sample-modpack.json with:

- name: human readable mod name
- file: the mod archive file name inside mods/
- version: mod version string
- url: official download URL (optional but recommended)

## Step 3: Validate the manifest

Open example/sample-modpack.json and verify that it is valid JSON and that
every file value matches an actual file in mods/.

## Step 4: Package and distribute

Zip the mods/ directory and the manifest file together. Share the archive
with players, or import it into a modpack launcher that supports custom
modpacks.

## Launching the modpack

Launch the modpack using the launcher appropriate for your target platform.
This repository does not include a start script; use the modpack loader
provided by Forge, Fabric, or NeoForge to load the pack.

## Configuration

Configuration files, if present, live in the repository root or in a config
directory. Edit them with a plain text editor and restart the modpack for
changes to take effect.

Back up configuration files before editing them so you can restore a working
configuration if needed.

## Troubleshooting

| Problem | Possible cause | Suggested fix |
| ------- | -------------- | ------------- |
| Modpack will not start | Missing dependencies | Install the dependencies listed in docs/getting-started.md |
| Mod fails to load | Wrong game version or loader | Check that the mod supports the game version and loader you installed |
| Configuration not applied | File not saved or wrong location | Confirm the file path matches the documented location |
| Missing library mod | Required dependency not installed | Add the library mod to mods/ and to the manifest as well |
| Performance issues | Insufficient resources | Allocate more memory or close other applications |
| Crash on startup | Faulty mod | Review the crash report in the game logs directory and remove the mod listed in the error |

If the problem persists, open an issue in the repository:
https://github.com/PritheshPoobalan/modpackpriprogoat/issues

## Keeping the modpack up to date

Pull the latest changes from the remote repository:

git pull origin main

Review any new or changed files, then restart the modpack.
