# Pi Agents

Personal agent package for `pi-subagents`.

Current contents:
- `scout` - bounded repository reconnaissance for low-complexity discovery and scope narrowing

## How it works

Pi does not natively discover package `agents/` directories.
This package ships a tiny extension that registers its local `agents/` folder with the `pi-subagents` package-agent registry at runtime.

That keeps the canonical agent definitions as Markdown files while making them discoverable from installed packages.

## Requirements

- `pi-subagents` must be installed in the same Pi environment.

## Install

Local development install:

```bash
pi install "<path-to-pi-agents>"
```

Project-local install:

```bash
pi install -l "<path-to-pi-agents>"
```

## Package layout

```text
pi-agents/
  agents/
    scout.md
  extensions/
    register-subagents.ts
```

## License

MIT. See `LICENSE`.
