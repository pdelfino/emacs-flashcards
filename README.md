# emacs-flashcards

![The Bookworm](https://upload.wikimedia.org/wikipedia/commons/thumb/9/99/Carl_Spitzweg_-_%22The_Bookworm%22.jpg/960px-Carl_Spitzweg_-_%22The_Bookworm%22.jpg)

*"The Bookworm" (c. 1850) by Carl Spitzweg — [Wikipedia](https://en.wikipedia.org/wiki/The_Bookworm_(painting))*

**Spaced repetition flashcards for learning Emacs -- built inside Emacs itself.**

## About

Emacs is tough to learn. The keybindings alone are a mountain, and there is always a faster, more elegant way to do something that you haven't discovered yet. This repository is a deck of flashcards designed to be drilled with [org-drill](https://orgmode.org/worg/org-contrib/org-drill.html), the spaced repetition system that runs inside Emacs via org-mode.

The deck is a plain `.org` file with special annotations. You can read it as-is -- org-mode's simple markup keeps the source comfortable to browse. But the real value comes from running `org-drill`, which turns each heading into a timed flashcard and schedules reviews using a spaced repetition algorithm.

There is nothing more like true Emacs hacking than using a spaced repetition tool *inside* Emacs to get better *at* Emacs.

## What the Deck Covers

The `emacs.org` file contains 98 exercises spanning:

- **Core keybindings** -- navigation, editing, killing, yanking, transposing
- **Org-mode** -- headings, lists, checkboxes, tables, links, clocking, export
- **Dired** -- file management, renaming, moving, navigating directories
- **Magit** -- status, staging, committing, rebasing, stashing, spin-off branches
- **Paredit** -- slurping, barfing, wrapping s-expressions
- **CIDER** -- Clojure REPL history, auto-complete
- **Flyspell** -- spell checking navigation and correction
- **Keyboard macros** -- recording, replaying, batching
- **Shell and terminal modes** -- differences between shell-mode, term-mode, and eshell

## How to Use

1. Clone the repo and open `emacs.org` in Emacs
2. Make sure [org-drill](https://orgmode.org/worg/org-contrib/org-drill.html) is installed (available via MELPA or straight.el)
3. Run `M-x org-drill`
4. Answer each card, rate your recall, and let the algorithm schedule your next review

```shell
git clone git@github.com:pdelfino/emacs-flashcards.git ~/projects/emacs-flashcards
```

## Requirements

- Emacs with org-mode
- [org-drill](https://orgmode.org/worg/org-contrib/org-drill.html)

## Further Resources

- [Mastering Emacs](https://www.masteringemacs.org/) (book)
- [System Crafters](https://www.youtube.com/c/SystemCrafters) YouTube channel -- especially [Emacs from Scratch](https://www.youtube.com/watch?v=74zOY-vgkyw&list=PLEoMzSkcN8oPH1au7H6B7bBJ4ZO7BXjSZ)
- [GNU Emacs refcards](https://www.gnu.org/software/emacs/refcards/)
- The built-in tutorial: `M-x help-with-tutorial`

## Contributing

Contributions are welcome. If you have flashcards for Emacs topics not yet covered, feel free to send a patch.
