# Modpack manifest format (flat format)

The manifest is a JSON file at the repository root, for example `modpack.json`.
Two complete examples are stored in the `example/` directory:
`example/modpack-manifest.json` (Fabric) and
`example/modpack-manifest-forge.json` (Forge). Field meanings are described
below. The repository also contains a nested-format example at
`example/sample-modpack.json`; choose one format and use it consistently.

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
