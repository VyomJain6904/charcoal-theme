# Charcoal

A deep-black grayscale theme with no hues — everything rendered in shades of gray.
Inspired by minimal dark terminal setups. Created by [Vyom Jain](https://github.com/VyomJain6904).

## Color Palette

| Role             | Hex       |
|------------------|-----------|
| Background       | `#0d0d0d` |
| Foreground       | `#c4c4c4` |
| Comments         | `#505050` |
| Strings          | `#909090` |
| Keywords         | `#e0e0e0` |
| Functions        | `#bcbcbc` |
| Variables        | `#acacac` |
| Numbers          | `#b4b4b4` |
| Types            | `#c8c8c8` |
| Operators        | `#787878` |

## Supported Tools

- **bat** — syntax-highlighting cat clone
- **Ghostty** — terminal emulator
- **OpenCode** — AI coding CLI

## Installation

### bat

```bash
mkdir -p "$(bat --config-dir)/themes"
curl -o "$(bat --config-dir)/themes/Charcoal.tmTheme" \
  https://raw.githubusercontent.com/VyomJain6904/charcoal-theme/main/bat/Charcoal.tmTheme
bat cache --build
```

Then add to `~/.config/bat/config`:
```
--theme="Charcoal"
```

### Ghostty

```bash
mkdir -p ~/.config/ghostty/themes
curl -o ~/.config/ghostty/themes/Charcoal \
  https://raw.githubusercontent.com/VyomJain6904/charcoal-theme/main/ghostty/Charcoal
```

Then add to `~/.config/ghostty/config`:
```
theme=Charcoal
```

Reload Ghostty with `Ctrl+Shift+,`.

### OpenCode

```bash
mkdir -p ~/.config/opencode/themes
curl -o ~/.config/opencode/themes/charcoal.json \
  https://raw.githubusercontent.com/VyomJain6904/charcoal-theme/main/opencode/charcoal.json
```

Then add to `~/.config/opencode/opencode.json`:
```json
{ "theme": "charcoal" }
```

## License

MIT © [Vyom Jain](https://github.com/VyomJain6904)
