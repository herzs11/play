# play

play is a TUI playground for your favorite programs, such as grep, sed and awk.

<p align="center">
    <picture>
      <source media="(prefers-color-scheme: dark)" srcset="docs/gopher.png">
      <source media="(prefers-color-scheme: light)" srcset="docs/gopher.png">
      <img alt="play" title="play" src="docs/gopher.png" width="300">
    </picture>
</p>

# Demo

![](docs/demo.gif)

It uses the excellent [tview](https://github.com/rivo/tview) library for the UI.

# Installation

```bash
$ git clone https://github.com/paololazzari/play
$ cd play
$ go build -o /usr/local/bin/
```

# Usage

```bash
./play <program>
```

## Key bindings

| Component       | Key           | Description |
|-----------------|---------------|-------------|
| Command Options      | `Tab`         | Move focus to positional arguments  |
| Command Options      | `Shift+Tab`   | Move focus to file picker |
| Command Options      | `Enter`       | Move focus to output |
| Positional Arguments | `Tab`         | Move focus to file picker |
| Positional Arguments | `Shift+Tab`   | Move focus to command options |
| Positional Arguments | `Enter`       | Move focus to output |
| Positional Arguments | `Ctrl+O`      | Open wide editor/Close wide editor |
| File picker          | `Tab`         | Move focus to command options |
| File picker          | `Shift+Tab`   | Move focus to positional arguments options |
| File picker          | `Ctrl+O`      | Open selected file/Close selected file | 
| Output               | `Esc`         | Move focus to previous component |