Overview
========

Purpose
-------

modpackpriprogoat holds modular pack components in one place so they can be
versioned, reviewed, and reused together. Each module is self-contained and
describes its own purpose, setup, and usage.

Repository layout
-----------------

- README.md          - project description and basic usage
- docs/              - project documentation
- example/           - example files for reference
- modules/           - modular pack components (create this directory when you
                       add your first module)

Adding a module
---------------

1. Create a directory under modules/ named after your module.
2. Place the module files inside that directory.
3. Add a README.md inside the module directory with:
   - module name and purpose
   - installation steps
   - configuration options
   - dependencies, if any
4. Commit the module and open a pull request.

Example
-------

See example/sample.modpack for a minimal module manifest example.

Guidelines
----------

- Do not delete existing content.
- Keep each module self-contained.
- Document every module with its own README.
- Use conventional commit messages (for example, feat:, fix:, docs:, chore:).