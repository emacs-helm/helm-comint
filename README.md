# helm-comint

Access Emacs command interpreter prompts through helm.

You can bind this as follows in .emacs:

``` emacs-lisp
(add-hook 'comint-mode-hook
          (lambda ()
              (define-key comint-mode-map (kbd "M-s f") 'helm-comint-prompts-all)))
```

Or as another example you can see how [Spacemacs uses
it](https://github.com/syl20bnr/spacemacs/blob/develop/layers/%2Btools/shell/funcs.el)
in 'spacemacs/helm-shell-history'.

helm-comint is written by Pierre Neidhardt <mail@ambrevar.xyz>. Removed from
helm v3.9.5 core and exists as a user contrib package.

See https://git.savannah.gnu.org/cgit/emacs.git/tree/lisp/comint.el
See also https://www.masteringemacs.org/article/comint-writing-command-interpreter
