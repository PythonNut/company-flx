company-flx
===========

[![MELPA](http://melpa.org/packages/company-flx-badge.svg)](http://melpa.org/#/company-flx)

This package adds fuzzy matching to company, powered by the sophisticated sorting heuristics in flx.

Usage
=====

To install, either clone this package directly, or execute <kbd>M-x</kbd> `package-install` <kbd>RET</kbd> `company-flx` <kbd>RET</kbd>.

After the package is installed, you can enable `company-flx` by adding the following to your init file:

```emacs
(with-eval-after-load 'company
  (company-flx-mode +1))
```

Use the variable `company-flx-limit` to control the number of candidates that are scored by `flx`. `flx` can be slow, and the default is set rather high, so if you experience lag, consider lowering the limit.

Some History
============

Crazy stuff simmers in my [`emacs-config`](https://github.com/PythonNut/emacs-config), and every once and a while, it's worth sharing. [This was no exception](https://github.com/PythonNut/emacs-config/blob/f1df3ac16410bfa72d88855325bd6c2de56f587b/modules/config-helm.el#L33#L89). It's been patiently evolving in my config for the better part of a year, and I think it's useful enough to benefit other people.

Also of interest is [company-mode/**company-mode** #47](https://github.com/company-mode/company-mode/issues/47).

Caveats
=======

This only works with the `company-capf` backend. Most sources use this backend, with the exception of the more advanced sources. Most backends should be re-written in terms of `completion-at-point-functions` eventually, although it's going to take a while.

The most important source that doesn't work is `company-dabbrev`.
