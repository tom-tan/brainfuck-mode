# brainfuck-mode.el

This library helps you to write brainfuck in Emacs.
This is also an example to define help document functions by using langdoc.

Requirement:
   langdoc.el

To use this package, add the following line to your `.emacs` file:
```emacs
    (require 'brainfuck-mode)
    ;; If you use brainfuck-mode for bf files
    (setq auto-mode-alist
          (append '(("\\.bf$" . brainfuck-mode))
                  auto-mode-alist))
```
brainfuck-mode highlights some keywords for usability.
By using `M-x eldoc-mode`, you can see the help string in minibuffer.
Also, by using `M-x bf-help-describe-symbol` (or C-c f), you can see
more documents for each command.
