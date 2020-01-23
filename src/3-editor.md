# The Editor

---

`apt install neovim`

---

Built-in documentation: `:help`

---

`:Tutor` if you want to practice your vim moves.

---

Also, check out [VIM Adventures](https://vim-adventures.com/).

---

## Motions

From normal mode:
- `w`: Move one word.
- `W`: Move one WORD (only whitespace is considered the delimiter).
- `b`: Go backwards one word.
- `B`: Go backwards one WORD.
- `%`: Move around delimiters (e.g., `()`).
- `f`: Move to the next matching character.
- `F`: Move to the previous matching character.
- `t`: Move right before the next maching character.
- `T`: Move right after the previous matching character.

---

## Motions (continued)
- `gg`: Go to start of file.
- `G`: Go to end of file.
- `^`: Go to start of line.
- `$`: Go to end of line.

---

## Modifiers

You can multiply a motion, for example:
- `2w`: Move two words.
- `4<down>`: Move down 4 lines.
- `3p`: Paste clipboard content 3 times.

---

## Actions

You can do other things than just move around. You can:
- `y`: Copy.
- `d`: Delete.
- `c`: Delete and go into insert mode.

---

For example:
- `dw`: delete a word
- `d2W`: delete two WORDs
- `yt"`: copy from the current line up to the quote.
- `yy`: copy the entire line.

---

Ok lets slow down a bit...

---

## Composition

You can combine commands together:

```
[action][modifier]<motion>
```

---

## Buffers

A buffer is an opened file.

---

- `:ls`: List buffers.
- `:bnext` / `:bn`: Move to the next buffer.
- `:bprevious` / `:bp`: Move to previous buffer.
- `:b<number>`: Move to buffer at corresponding index.

---

## Windows

Windows are a view on a buffer.

---

- `Ctrl-ws`: Create a horizontal split.
- `Ctrl-wv`: Create a vertical split.
- `Ctrl-wq`: Close the current window.
- `Ctrl-ww`: Iterate over the current windows.
- `w<arrow>`: Move to the window in the specified direction.

---

## Plugins

---

[Vim-Plug](https://github.com/junegunn/vim-plug) is a simple package manager.

To install:
```
curl -fLo ~/.vim/autoload/plug.vim --create-dirs \
    https://raw.githubusercontent.com/junegunn/vim-plug/master/plug.vim
```

---

With a simple vimrc:
```vim
call plug#begin('~/.vim/plugged')
Plug 'morhetz/gruvbox'
call plug#end()

silent! colorscheme gruvbox
set background=dark
```

---

## File Tree
Personally, I use NERDTree:

```vim
Plug 'preservim/nerdtree'
```

If you find `:NERDTree` to be too long to write, you can create an abbreviation:
```vim
cabbrev t NERDTree
```

---

## File Search

Fairly similar to what most editors offer:
```vim
Plug 'ctrlp/ctrlp.vim'
```

---

## Git Integration

```vim
Plug 'tpope/vim-fugitive'
```

---

## Language Integration

This is where things can get hairy with plugins.

---

For most languages, syntax support works out of the box. For JSX support,
you'll want to add another plugin though:

```vim
Plug 'pangloss/vim-javascript'
```

---

Linter is fairly simple, you just need one plugin to handle all languages:
```vim
Plug 'dense-analysis/ale'
```

---

Code completion / jump to definition is extra hairy. There are several options
out there, but generally speaking YouCompleteMe has been the plugin of choice.

---

Questions?
