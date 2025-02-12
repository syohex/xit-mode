# xit-mode

[x]it! is a plain-text file format for todos and check lists. This is an Emacs major mode that gives highlighting for .xit files.

![Screenshot](https://raw.githubusercontent.com/ryanolsonx/xit-mode/main/screenshot.png "Screenshot of Emacs [x]it!")

## Installation

As this is WIP, it's not available on Melpa. When it's more complete, it'll be in Melpa. So for now, to use this, you'll need to:

### 1. Download the package

```bash
cd ~/.emacs.d/
git clone https://github.com/ryanolsonx/xit-mode
```

### 2. Load it in Emacs

In your .emacs or init.el:

```elisp
(load "~/.emacs.d/xit-mode/xit-mode.el")
(require 'xit-mode)
```

## Key bindings

- `C-c C-n` (`M-x xit-new-item`) : Create a new open item
- `C-c C-o` (`M-x xit-open-item`) : Set an item as open (`[ ]`)
- `C-c C-d` (`M-x xit-checked-item`) : Set an item as checked (`[x]`)
- `C-c C-p` (`M-x xit-ongoing-item`) : Set an item as ongoing (`[@]`)
- `C-c C-a` (`M-x xit-obsolete-item`) : Set an item as obsolete (`[!]`)
- `C-c C-C` (`M-x xit-state-cycle-item `) : Cycle through the different states (`open` -> `ongoing` -> `checked` -> `obsolete`)
- `C-c C-<up>` (`M-x xit-inc-priority-item`) : Increase the priority by adding a `!`
- `C-c C-<down>` (`M-x xit-dec-priority-item`) : Decrease the priority by removing a `!` or a `.`

## Customizable faces

Here is the list of the faces used in the `xit-faces` group:

- `xit-open-checkbox-face`
- `xit-open-description-face`
- `xit-checked-checkbox-face`
- `xit-checked-description-face`
- `xit-ongoing-checkbox-face`
- `xit-ongoing-description-face`
- `xit-obsolete-checkbox-face`
- `xit-obsolete-description-face`
- `xit-priority-face`
- `xit-tag-face`
