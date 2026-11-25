# Getting started

This guide walks you through setting up the modpackpriprogoat modpack from scratch.

## Step 1: Clone the repository

Open a terminal and run:

git clone https://github.com/PritheshPoobalan/modpackpriprogoat.git
cd modpackpriprogoat

## Step 2: Review the repository layout

After cloning, the repository contains:

- README.md — project overview
- docs/ — documentation files
- Any modpack configuration files and scripts present in the repository

Do not delete existing content when adding new files.

## Step 3: Install dependencies

Check the target platform documentation for the installer or package manager
required by the modpack. Install any required dependencies before proceeding.

If a setup script is included in the repository, run it from the repository root:

./setup.sh

Otherwise, follow the platform-specific installation steps described in
docs/usage.md.

## Step 4: Verify the installation

Run the modpack or its launcher and confirm it starts without errors. If you
encounter problems, see the troubleshooting section in docs/usage.md.

## Next steps

- Read docs/usage.md for usage instructions and configuration options.
- Read docs/contributing.md if you plan to contribute changes.
