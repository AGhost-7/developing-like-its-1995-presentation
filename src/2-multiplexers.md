# Multiplexers

---

Who knows what a multiplexer is?

---

`apt install tmux`

---

There are two kinds of objects:
- Window: A tab in tmux speal.
- Pane: Any sort of split within a tab

---

All keybindings are sitting behind a "prefix". Default is Ctrl-B.

---

- `Prefix-C`: Create window.
- `Prefix-"`: Horizontal split.
- `Prefix-%`: Vertical split.
- `Prefix-X`: Close pane.
- `Prefix-<number>`: Jump to window.
- `Prefix-Z`: Zoom Pane / Hide other panes not focused.

---

Enable mouse: `Prefix-:` and type `mouse on`.

---

Tmux is useful on servers as well.

---

- `tmux new -s foobar`: create a new session named "foobar".
- `Prefix-D`: Detach from tmux.
- `tmux attach -t foobar`: attach to named session.

---

Questions?
