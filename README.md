# Custom Icon Shell

A simple macOS utility for changing application and folder icons from the terminal.

This project is a starter tool. It lets you use commands like:

```bash
seticon Finder ./icons/finder.icns
seticon Terminal ./icons/terminal.icns
seticon ~/Desktop/MyFolder ./icons/folder.icns
```

The script uses macOS Finder and `osascript` to apply a custom icon.

## What is in this repo

- `bin/seticon` — main command-line tool
- `icons/` — example icon files and folders
- `examples/targets.txt` — sample app targets
- `README.md` — usage instructions

## Install

```bash
mkdir -p ~/.local/bin
cp bin/seticon ~/.local/bin/seticon
chmod +x ~/.local/bin/seticon
```

Add it to your PATH if needed:

```bash
export PATH="$HOME/.local/bin:$PATH"
```

## Usage

```bash
seticon <target> <icon-file>
```

Examples:

```bash
seticon Finder ./icons/finder.icns
seticon /Applications/Utilities/Terminal.app ./icons/terminal.icns
seticon ~/Desktop/MyFolder ./icons/folder.icns
seticon safari ./icons/safari.icns
```

## Notes

- Works on macOS only
- Best with `.icns` files
- PNG/JPG files are auto-converted with `sips`

## License

MIT
