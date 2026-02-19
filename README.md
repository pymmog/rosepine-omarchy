# Omarchy Rosé Pine Theme

A [Rosé Pine](https://rosepinetheme.com) color scheme for [Omarchy](https://omarchy.com), available in three variants:

| Variant | Description |
|---------|-------------|
| **default** | Rosé Pine — the original dark theme |
| **moon** | Rosé Pine Moon — a softer dark theme |
| **dawn** | Rosé Pine Dawn — a warm light theme |

## Installation

### Option 1: Clone the repo (recommended)

```bash
git clone https://github.com/you/rosepine-omarchy.git /tmp/rosepine-omarchy
```

Copy your preferred variant to the Omarchy themes directory:

```bash
# default (dark)
cp -r /tmp/rosepine-omarchy/default ~/.config/omarchy/themes/rosepine

# moon
cp -r /tmp/rosepine-omarchy/moon ~/.config/omarchy/themes/rosepine-moon

# dawn (light)
cp -r /tmp/rosepine-omarchy/dawn ~/.config/omarchy/themes/rosepine-dawn
```

### Option 2: Clone a single variant (submodule)

Each variant is also available as a standalone repo:

```bash
git clone https://github.com/you/rosepine-omarchy-default.git ~/.config/omarchy/themes/rosepine
git clone https://github.com/you/rosepine-omarchy-moon.git ~/.config/omarchy/themes/rosepine-moon
git clone https://github.com/you/rosepine-omarchy-dawn.git ~/.config/omarchy/themes/rosepine-dawn
```

### Option 3: curl individual files

```bash
VARIANT="default"  # or "moon" or "dawn"
DEST="$HOME/.config/omarchy/themes/rosepine"
BASE="https://raw.githubusercontent.com/you/rosepine-omarchy/main/$VARIANT"

mkdir -p "$DEST"
for f in colors.toml btop.theme neovim.lua vscode.json waybar.css icons.theme; do
  curl -sL "$BASE/$f" -o "$DEST/$f"
done
```

## Theme files

Each variant includes:

- `colors.toml` — terminal colors
- `btop.theme` — btop system monitor
- `neovim.lua` — Neovim colorscheme (LazyVim)
- `vscode.json` — VS Code theme extension
- `waybar.css` — Waybar foreground/background
- `icons.theme` — icon theme

## Credits

- [Rosé Pine](https://rosepinetheme.com) for the color palette
- [Omarchy](https://omarchy.com) for the desktop environment
