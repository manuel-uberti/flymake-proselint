# flymake-proselint

This package makes it possible to use [proselint](http://proselint.com/) with the Emacs built-in Flymake.

## Getting started

`flymake-proselint` is not listed on ELPA nor MELPA. If you want to try it, you
can use [`straight.el`](https://github.com/raxod502/straight.el) to install it:

``` emacs-lisp
(straight-use-package
  '(flymake-proselint :host github :repo "manuel-uberti/flymake-proselint"))
```

Then you just need to activate in the modes you want your prose to be checked:

``` emacs-lisp
(add-hook 'markdown-mode-hook #'flymake-proselint-setup)
```

