# Pre-commit hooks

Please see the [pre-commit](https://pre-commit.com/) page for information on how to install this.

## Hooks

There are currently two hooks:

* ts-no-console-log
    * Reacts to console.(info|log) calls and rejects them
* ts-no-focus-test
    * Reacts to \[fx\](describe|it) calls in .spec.ts / spec.js files
* ts-accessing-window
    * Reacts to attempts trying to write something to the window object
