# Charcoal

A deep-black grayscale theme with no hues — everything rendered in shades of gray.
Inspired by minimal dark terminal setups. Created by [Vyom Jain](https://github.com/VyomJain6904).

## Color Palette

| Role             | Hex       |
|------------------|-----------|
| Background       | `#0d0d0d` |
| Foreground       | `#d4d4d4` |
| Comments         | `#686868` |
| Strings          | `#aaaaaa` |
| Keywords         | `#eeeeee` |
| Functions        | `#cccccc` |
| Variables        | `#c0c0c0` |
| Numbers          | `#c8c8c8` |
| Types            | `#d8d8d8` |
| Operators        | `#8e8e8e` |

## Supported Tools

- **bat** — syntax-highlighting cat clone
- **Ghostty** — terminal emulator
- **OpenCode** — AI coding CLI
- **Neovim** — full colorscheme plugin → [charcoal.nvim](https://github.com/VyomJain6904/charcoal.nvim)

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

### Neovim

Install via lazy.nvim:

```lua
{
  'VyomJain6904/charcoal.nvim',
  priority = 1000,
  config = function()
    vim.cmd.colorscheme('charcoal')
  end,
}
```

Full plugin: [charcoal.nvim](https://github.com/VyomJain6904/charcoal.nvim)

## License

MIT © [Vyom Jain](https://github.com/VyomJain6904)
