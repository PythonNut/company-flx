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

Some History
============

Crazy stuff simmers in my [`emacs-config`](https://github.com/PythonNut/emacs-config), and every once and a while, it's worth sharing. [This was no exception](https://github.com/PythonNut/emacs-config/blob/f1df3ac16410bfa72d88855325bd6c2de56f587b/modules/config-helm.el#L33#L89). It's been patiently evolving in my config for the better part of a year, and I think it's useful enough to benefit other people.

Also of interest is [company-mode/**company-mode** #47](https://github.com/company-mode/company-mode/issues/47).
