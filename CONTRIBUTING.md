# Contributing

We welcome contributions to improve the theme generator and add new palettes.

## How to Contribute

1. Fork the repository.
2. Create a feature branch: `git checkout -b feature/my-feature`.
3. Make your changes.
4. Run the generator to verify the output is valid: `cd labs && python3 generate_themes.py`.
5. Commit and push your branch.
6. Open a pull request describing the change.

## Adding a New Theme

1. Add your ANSI 16-color palette to `colors.md` using the existing format (JSON block with `color0` through `color15`, `background`, and `foreground`).
2. Add the corresponding entry to the `THEMES` dict in `labs/generate_themes.py`.
3. Run the generator to produce the `.xccolortheme` file.
4. Commit both the updated `colors.md` and the new file in `themes/`.

## Modifying the Color Mapping

The ANSI-to-Xcode syntax mapping is defined in the `SYNTAX_MAP` list inside `labs/generate_themes.py`. Adjust it if you believe a different token assignment produces better highlighting.

## Code Style

- Python: follow PEP 8.
- Shell scripts: use `#!/bin/bash` and shellcheck-clean code.
- Documentation: all text in English, no emojis, use HTML `<div align="center">` for centered titles.

## Review Process

All pull requests are reviewed for correctness, visual quality of the generated themes, and adherence to the project conventions.
