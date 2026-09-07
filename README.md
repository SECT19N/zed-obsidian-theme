# Obsidian Theme for Zed

A Zed theme inspired by the [Obsidian theme for Notepad++](https://notepad-plus-plus.org/), [nickc01's VS Code port](https://github.com/nickc01/Obsidian-Theme-VSCode), and the [Vercel theme for Zed](https://github.com/NathanBrodin/zed-vercel-theme).

Six variants built from one color language: a signature green accent (`#93c763`), a mauve alternative, warm gold highlights, and a **Soft** version of each for anyone who finds the originals too contrasty.

## Variants

| Theme                    | Accent          | Editor background | Text contrast |
| ------------------------ | --------------- | ----------------- | ------------- |
| **Obsidian Dark**        | green `#93c763` | `#0a0a0a`         | 16.9:1        |
| **Obsidian Dark Soft**   | green `#93c763` | `#1e1e1e`         | 10.7:1        |
| **Obsidian Purple**      | mauve `#c6a0f6` | `#0b0a0f`         | 16.8:1        |
| **Obsidian Purple Soft** | mauve `#c6a0f6` | `#1f1d26`         | 10.7:1        |
| **Obsidian Light**       | green `#5a8f2e` | `#ffffff`         | 17.9:1        |
| **Obsidian Light Soft**  | green `#5a8f2e` | `#faf6ee`         | 12.2:1        |

The **Soft** variants keep every accent hue but lift the backgrounds and ease off the
foreground, trading the stark look for something easier on the eyes over a long session.
Obsidian Light Soft swaps white for warm paper and a warm near-black. The **Purple**
variants tint the neutrals toward mauve at the same luminance, so they match their green
counterparts' contrast exactly.

## Screenshots

### Obsidian Dark

![Obsidian Dark theme in Zed](assets/obsidian-dark.png)

### Obsidian Light

![Obsidian Light theme in Zed](assets/obsidian-light.png)

> **Adding screenshots:** Save your captures as `assets/obsidian-dark.png` and `assets/obsidian-light.png`. For best results, use a wide aspect ratio (e.g. 1920×1080) showing the editor with syntax highlighting, the sidebar, and the status bar.

## Features

- **Six variants** — dark, purple, and light, each in a standard and a low-contrast Soft version
- **Syntax highlighting** — keywords and constructors in the accent hue, functions in purple (dark) / pink (purple) / neutral (light), strings in gold, types in blue
- **Terminal colors** — full ANSI palette tuned to match the editor
- **UI polish** — accent-colored focus borders, search match highlights, and version-control colors

## Color Palette

| Role                     | Dark      | Purple    | Light     |
| ------------------------ | --------- | --------- | --------- |
| Background               | `#0a0a0a` | `#0b0a0f` | `#f5f5f5` |
| Foreground               | `#ededed` | `#ededed` | `#171717` |
| Accent (keywords, links) | `#93c763` | `#c6a0f6` | `#93c763` |
| Functions                | `#B477CF` | `#f5c2e7` | `#171717` |
| Strings / constants      | `#efc210` | `#efc210` | `#efc210` |
| Types / hints            | `#678cb1` | `#678cb1` | `#678cb1` |
| Comments                 | `#666666` | `#666666` | `#999999` |

Git and diagnostic colors stay semantic across every variant — added lines are green even in
the purple themes.

## Installation

### From the Zed Extension Gallery

Once published to the [Zed extension registry](https://github.com/zed-industries/extensions):

1. Open the Extensions panel (`Ctrl+Shift+X` / `Cmd+Shift+X`)
2. Search for **Obsidian Theme**
3. Click **Install**

### From source (dev extension)

1. Clone this repository:

   ```bash
   git clone https://github.com/SECT19N/zed-obsidian-theme.git
   cd zed-obsidian-theme
   ```

2. In Zed, open the Extensions panel (`Ctrl+Shift+X` / `Cmd+Shift+X`)
3. Click **Install Dev Extension**
4. Select the cloned `zed-obsidian-theme` directory

The theme loads immediately — no build step required.

## Usage

1. Open the command palette (`Ctrl+Shift+P` / `Cmd+Shift+P`)
2. Run **theme selector: toggle**
3. Choose any of the six **Obsidian** variants

Zed will remember your selection across sessions.

## Project Structure

```
zed-obsidian-theme/
├── extension.toml      # Extension manifest
├── themes/
│   └── obsidian.json   # Theme definitions (all six variants)
├── assets/             # Screenshots (add your own)
│   ├── obsidian-dark.png
│   └── obsidian-light.png
└── LICENSE
```

## Credits

- [Obsidian Theme](https://github.com/nickc01/Obsidian-Theme-VSCode) by nickc01 — original color scheme
- [Vercel Theme for Zed](https://github.com/NathanBrodin/zed-vercel-theme) — structural inspiration for the Zed theme format

## License

[MIT](LICENSE) © 2026 [SECT19N](https://github.com/SECT19N)

## Contributing

Issues and pull requests are welcome. If you open a PR that changes colors, please include before/after screenshots in `assets/`.
