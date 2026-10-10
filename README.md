# custom-icon-shell

A macOS utility for setting custom application and folder icons.

## Install

```bash
mkdir -p ~/.local/bin
cp bin/seticon ~/.local/bin/seticon
chmod +x ~/.local/bin/seticon
```

Add to PATH:

```bash
export PATH="$HOME/.local/bin:$PATH"
```

Then you can use:

```bash
/seticon finder ./icons/finder.icns
/seticon Terminal ./icons/terminal.icns
```

## Usage

```bash
/seticon <target> <icon-file>
```

## Notes

- macOS only
- `.icns` works best
- PNG/JPG are auto-converted

## License

MIT
