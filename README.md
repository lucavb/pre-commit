# Pre-commit hooks

A set of pre-commit hooks that are used by me.

## How to use

Add the following to your .pre-commit-config.yaml file

```yaml
  - repo: https://github.com/lucavb/pre-commit
    rev: v0.0.2 # Pick the current tag
    hooks:
      - id: ts-debugger
      # -   id: ...
```


For further information see the [pre-commit](https://pre-commit.com/) page.

## Hooks

There are currently two hooks:

* ts-no-console-log
    * Reacts to console.(info|log) calls and rejects them
* ts-no-focus-test
    * Reacts to \[fx\](describe|it) calls in .spec.ts / spec.js files
* ts-accessing-window
    * Reacts to attempts trying to write something to the window object
* ts-debugger
    * Reacts to calls to the debugger

Unless otherwise specified, the hooks target .ts files.