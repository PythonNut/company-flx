`company-flx`
=============

This package adds fuzzy matching to company, powered by the sophisticated sorting heuristics in flx.

Usage
=====

To install, either clone this package directly, or execute <kbd>M-x</kbd> `package-install` <kbd>RET</kbd> `company-flx` <kbd>RET</kbd>.

After the package is installed, you can enable `company-flx` by adding:

```emacs
(with-eval-after-load 'company
  (company-flx-mode +1))
```

To your init file.
