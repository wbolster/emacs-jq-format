jq-format.el
============

This Emacs package provides a [reformatter](https://github.com/purcell/reformatter.el) for [json](https://www.json.org/) and [jsonlines](http://jsonlines.org/) files using the `jq` utility.

Installation
------------

Make sure [jq](https://stedolan.github.io/jq/) is installed on your sytem.

Install the [jq-format Melpa package](https://melpa.org/#/jq-format) using:

```
M-x package-install RET jq-format RET
```

If you use [use-package](https://github.com/jwiegley/use-package), use something like this:

``` elisp
(use-package jq-format
  :demand t
  :after json-mode)
```

Usage
-----

Use one of these commands via `M-x` or bind them to a key:

- `jq-format-json-buffer`
- `jq-format-json-region`
- `jq-format-json-on-save-mode`

A similar set of commands is avaiable for _jsonlines_ data:

- `jq-format-jsonlines-buffer`
- `jq-format-jsonlines-region`
- `jq-format-jsonlines-on-save-mode`

See the [reformatter](https://github.com/purcell/reformatter.el) documentation for more information

Configuration
-------------

This package deliberately has minimal configuration. Use `M-x customize-group RET jq-format` or change these variables in your `init.el`:

- `jq-format-command`
- `jq-format-sort-keys`
- `jq-format-extra-args`

License
-------

3-clause BSD. Copyright © 2019 wouter bolsterlee.

Credits
-------

wouter bolsterlee. wbolster.

https://github.com/wbolster on github. star my repos. fork them. and so on.

https://twitter.com/wbolster on twitter. follow me. or say hi.
