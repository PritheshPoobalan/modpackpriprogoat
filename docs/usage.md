# Usage

This document describes how to use the modpackpriprogoat modpack after
installation.

## Launching the modpack

Launch the modpack using the launcher or start script appropriate for your
platform. If a start script is included in the repository, run it from the
repository root:

./start.sh

Otherwise, use the modpack launcher provided by the target platform.

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
| Configuration not applied | File not saved or wrong location | Confirm the file path matches the documented location |
| Performance issues | Insufficient resources | Allocate more memory or close other applications |

If the problem persists, open an issue in the repository:
https://github.com/PritheshPoobalan/modpackpriprogoat/issues

## Keeping the modpack up to date

Pull the latest changes from the remote repository:

git pull origin main

Review any new or changed files, then restart the modpack.
