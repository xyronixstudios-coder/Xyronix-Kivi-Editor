# Xyronix Kivi Editor

Modern, modeless (nano-style) terminal text editor written in Go.

**Author:** Eren Mut  
**Studio:** Xyronix Studios  
**Version:** 1.0.7  
**Binary:** `kivi`  
**Module:** `xyronix-kivi-editor`

## Features

- Modeless editing (no hjkl, no modes)
- Kivi-green theme tuned for dark terminals
- Mouse: click, drag to select, wheel to scroll
- Auto-copy on selection release (OSC 52)
- UTF-8 / multi-language support
- Live window resize
- Nano-compatible keybindings

## Quick install

    git clone <repo> xyronix-kivi
    cd xyronix-kivi
    ./install.sh

The installer detects your distribution (Debian, Arch, Fedora, openSUSE,
Alpine) and installs Go if needed.

## Manual build

    make
    sudo make install

## Usage

    kivi [file]
    kivi --version
    kivi --help

## Keybindings

| Key | Action |
|-----|--------|
| `Ctrl+O` | Save |
| `Ctrl+X` | Exit (asks if modified) |
| `Ctrl+R` | Open file |
| `Ctrl+W` | Search |
| `Ctrl+K` | Cut line or selection |
| `Ctrl+U` | Paste |
| `Ctrl+C` | Copy selection |
| `Ctrl+A` | Home |
| `Ctrl+E` | End |
| `Ctrl+Y` | Page up |
| `Ctrl+V` | Page down |
| `Ctrl+G` | Help |

## Mouse

- Click to place cursor
- Drag to select text
- Release to copy selection to clipboard
- Wheel to scroll

## License

MIT
