# Glass Dracula for Zed

Glass Dracula is the Zed theme family I use and maintain. It combines
Dracula-inspired contrast with custom palettes across four carefully tuned
dark and light variants, including opaque and blurred surfaces.

## Themes

| Theme | Mode | Surface | Best for |
| --- | --- | --- | --- |
| **Dracula Dark Vivid Black** | Dark | Opaque | Pure black with a high-saturation custom neon palette |
| **Dracula Glass** | Dark | Blurred | Unified dark glass with a softer neon palette |
| **Dracula Light Vivid White** | Light | Opaque | Crisp white with high-contrast custom syntax colors |
| **Dracula Light Glass** | Light | Blurred | Unified Apple-neutral translucent glass |

My current Zed setup uses **Dracula Light Glass** in light mode and
**Dracula Dark Vivid Black** in dark mode:

```json
{
  "theme": {
    "mode": "light",
    "light": "Dracula Light Glass",
    "dark": "Dracula Dark Vivid Black"
  }
}
```

## Design

All four variants share the same semantic syntax language, so code remains
visually consistent when switching modes:

- rose for keywords and JSX tags
- green for functions and methods
- cyan for types, properties, members, and constructors
- violet for constants, enums, numbers, and variants
- amber for strings
- orange for parameters and Rust lifetimes
- neutral gray for punctuation and comments

The opaque variants prioritize predictable contrast. The Glass variants use
native blurred surfaces while keeping editor text fully opaque and readable.
The themes are tuned for Rust, React/React Native, Flutter, and other
Tree-sitter- and LSP-powered language modes.

For the most complete language-aware highlighting, combine Tree-sitter syntax
highlighting with LSP semantic tokens:

```json
{
  "semantic_tokens": "combined"
}
```

## Install for Development

In Zed, run `zed: install dev extension` from the command palette and select
this repository.

For direct local testing on Windows, copy the files from `themes/` to:

```text
%APPDATA%\Zed\themes
```

Reload Zed after replacing a theme file.

## Extension Metadata

- ID: `glass-dracula`
- Version: `0.3.0`
- Author: `BennyWu`
- Repository: <https://github.com/Aniu456/glass-dracula>

## License

Released under the [MIT License](LICENSE).
