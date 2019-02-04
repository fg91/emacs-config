## General
* Get help with function `C-h f`
* Describe key: `C-h k`
* `view-lossage` shows the history of commands

## Buffers
* Open a new file with `C-x C-f` creates a new buffer
* Switch between buffers `C-x b` (and enter name if not the one suggested or `?` for more info)
* Create a new buffer with a name `C-x b` and enter name
* Kill a buffer `C-x k`
* List all buffers `C-x C-b`
* `ibuffer` (bound to `C-x C-b`): mark buffers for deletion with `d` and execute with `x`.

## Packages
* `M-x package-refresh-contents` to reload packages
* Instead of re-opening emacs after editing `.emacs` do `C-x C-e` or try `revert-buffer`

### package `try`
* `M-x try` and package name let's you try packages without installing them


## Org-mode
* Adding a link `C-c C-l`
* Move levels up and down `M-up`
* `#+STARTUP: showall` at beginning of `.org` document to avoid showing the collapsed view on startup

## Elisp
* Everything in parenthesis is a function: `(+ 2 3)` would mean *run the + function on 2 and 3* (run with `eval-last-sexp` or `C-x C-e`)
* Set variable `(setq v 100)`. You could now `(+ v v)` and get the result with `C-x C-e` or `C-j`
* `C-a` calls `(move-beginning-of-line nil)` and you could get the same effect runnig `C-x C-e` on this!!!
* `C-p` is equiv to `(previous-line)` and `(previous-line 5)` would jump 5 lines up