# Glass Dracula for Zed

Glass Dracula is the Zed theme family I use and maintain. It combines the
familiar Dracula accent palette with four carefully tuned dark, light, opaque,
and blurred variants.

## Themes

| Theme | Mode | Surface | Best for |
| --- | --- | --- | --- |
| **Dracula Dark Vivid Black** | Dark | Opaque | OLED displays and maximum contrast |
| **Dracula Glass** | Dark | Blurred | A softer, violet-tinted dark workspace |
| **Dracula Light Vivid White** | Light | Opaque | A crisp, high-contrast light workspace |
| **Dracula Light Glass** | Light | Blurred | A softer translucent light workspace |

My current Zed setup uses **Dracula Light Vivid White** in light mode and
**Dracula Glass** in dark mode:

```json
{
  "theme": {
    "mode": "light",
    "light": "Dracula Light Vivid White",
    "dark": "Dracula Glass"
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
- Version: `0.2.0`
- Author: `BennyWu`
- Repository: <https://github.com/Aniu456/glass-dracula>

## License

Released under the [MIT License](LICENSE).
