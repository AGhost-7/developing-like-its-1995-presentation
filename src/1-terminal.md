# Developing Like It's 1995

---

# The Terminal

Something that everyone is familiar with, but how well?

---

Readline is used by:
- bash
- REPLs
- Interactive command line tools such as psql

---

## Stuff that works everywhere

---

Actually before we start...

---

If you're using iTerm2, you will need to change settings for some of the shortcuts to work:
- Open up your default terminal profile
- Go to "Keys" tab
- Set Option to map to "Esc+"

---

- Ctrl-E: Move to the end of the line.
- Ctrl-A: Move to the start of the line.

---

Meta = Alt / Option

---

- Meta-F: Move forward one word
- Meta-B: Move backard on word

---

- Ctrl-W: Delete previous word
- Meta-D: Delete the next word
- Ctrl-K: Delete everything forward
- Ctrl-U: Delete everything backwards

---

- Ctrl-R: Search history
- Ctrl-L: Clear the screen

---

Want more? `man readline`

---

## Jobs

---

You can control applications that are running in your shell.

---

`jobs` command shows you what processes were run in your shell.

---

You can "pause" a program with Ctrl-Z. Resume with `fg` command.

---

## And...
The rest is knowing your programs as well as customizing your shell for
improved productivity.
