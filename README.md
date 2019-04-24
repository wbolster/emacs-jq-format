json-reformatter-jq.el
======================

This Emacs package provides a [reformatter](https://github.com/purcell/reformatter.el) for [json](https://www.json.org/) and [jsonlines](http://jsonlines.org/) files using the `jq` utility.

Installation
------------

Make sure [jq](https://stedolan.github.io/jq/) is installed on your sytem.

Install the [json-reformatter-jq Melpa package](https://melpa.org/#/json-reformatter-jq) using:

```
M-x package-install RET json-reformatter-jq RET
```

If you use [use-package](https://github.com/jwiegley/use-package), use something like this:

``` elisp
(use-package json-reformatter-jq
  :demand t
  :after json-mode)
```

Usage
-----

Use one of these commands via `M-x` or bind them to a key:

- `json-reformatter-jq-buffer`
- `json-reformatter-jq-region`
- `json-reformatter-jq-on-save-mode`

A similar set of commands is avaiable for _jsonlines_ data:

- `jsonlines-reformatter-jq-buffer`
- `jsonlines-reformatter-jq-region`
- `jsonlines-reformatter-jq-on-save-mode`

See the [reformatter](https://github.com/purcell/reformatter.el) documentation for more information

Configuration
-------------

This package deliberately has minimal configuration. Use `M-x customize-group RET json-reformatter-jq` or change these variables in your `init.el`:

- `json-reformatter-jq-command`
- `json-reformatter-jq-sort-keys`
- `json-reformatter-jq-extra-args`

License
-------

3-clause BSD. Copyright © 2019 wouter bolsterlee.

Credits
-------

wouter bolsterlee. wbolster.

https://github.com/wbolster on github. star my repos. fork them. and so on.

https://twitter.com/wbolster on twitter. follow me. or say hi.
