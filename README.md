# Glass Dracula for Zed

A refined Dracula-inspired theme family by **BennyWu**, designed around one
consistent syntax language with opaque and softly blurred dark and light UI
variants.

## Included Themes

- **Dracula Dark Vivid Black** — OLED-oriented opaque black
- **Dracula Glass** — violet-tinted blurred dark surfaces
- **Dracula Light Vivid White** — crisp porcelain-white editor
- **Dracula Light Glass** — softly blurred light surfaces

## Design System

All four variants share the same semantic color roles so code structure remains
stable when switching between light and dark mode. Neutral punctuation and
muted comments keep dense Rust, React/React Native, and Flutter code calm while
preserving familiar Dracula accents:

- rose for keywords and JSX tags
- green for functions and methods
- cyan for types, properties, members, and constructors
- violet for constants, enums, numbers, and variants
- amber for strings
- orange for parameters and Rust lifetimes
- neutral gray for punctuation and comments

The opaque variants prioritize predictable contrast. The Glass variants add
translucent surfaces and native blur while keeping editor text fully opaque.

For the best language-aware highlighting, enable Tree-sitter and LSP semantic
tokens together in Zed settings:

```json
{
  "semantic_tokens": "combined"
}
```

## Extension Metadata

- `id`: `glass-dracula`
- `name`: `Glass Dracula`
- `version`: `0.2.0`
- `repository`: `https://github.com/Aniu456/glass-dracula`

## Local Test

Use `zed: install dev extension` and select this repository, or copy the JSON
files from `themes/` into `%APPDATA%\Zed\themes` on Windows. Reload Zed after
updating local theme files.

## Publish

For public Zed distribution, submit/update this extension through the Zed extensions registry workflow.
