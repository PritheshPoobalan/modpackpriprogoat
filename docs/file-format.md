# Modpack manifest format

The manifest is a JSON file named `modpack.json` at the repository root. A complete example is stored at `example/modpack-manifest.json`. Field meanings are described below.

## Top-level fields

- `name` (string): pack name.
- `game_version` (string): Minecraft version the pack targets.
- `loader` (string): mod loader used by the pack, for example `fabric`, `forge`, or `neoforge`.
- `loader_version` (string): loader version, optional.
- `mods` (array): list of mod objects.

## Mod object fields

- `id` (string, required): mod identifier.
- `name` (string, required): display name.
- `version` (string, required): mod version.
- `loader` (string, optional): overrides the pack loader for this mod.
- `side` (string, optional): `client`, `server`, or `both`. Defaults to `both`.
- `required` (boolean, optional): whether the pack fails to load without this mod. Defaults to true.

## Example

See `example/modpack-manifest.json` for a complete example file.
