# rope-cli
A single uv-runnable CLI for basic move/rename refactoring operations in Python missing from all LSPs.

## Install

- Install uv (https://docs.astral.sh/ruff/installation/)
- Either download the script to your ~/.local/bin and chmod+x, or point uv run directly at it.

## How to use

```
❯ rope-cli
Usage: rope-cli [OPTIONS] COMMAND [ARGS]...

  CLI tool for Python refactoring operations.

Options:
  --help  Show this message and exit.

Commands:
  move-module    Move a Python module to a different package.
  move-symbol    Move a Python symbol from one module to another.
  rename-module  Rename a Python module.
```

## Why?

I use Helix as my editor – I love it – but refactoring can be a pain as compared to Pycharm/VS Code. For whatever reason, no LSP for Python today offers code actions for renaming/moving symbols or modules. This CLI tool takes care of that. It's still not great, but it's better than needing to fire up Pycharm just to move a function to a different module.

## Credits

- [Rope](https://github.com/python-rope/pylsp-rope), which does all the heavy lifting.
- Claude Sonnet 3.5 for giving me a working implementation in a minute.
