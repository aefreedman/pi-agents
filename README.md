# Pi Agents

Reusable agent definitions for Pi's `pi-subagents` package.

## Contents

- `scout` - bounded repository reconnaissance for low-complexity discovery and scope narrowing

## How it works

Pi does not natively discover package `agents/` directories. This package ships a small extension that registers its local `agents/` folder with the `pi-subagents` package-agent registry at runtime.

That keeps canonical agent definitions as Markdown files while making them discoverable from installed packages.

## Requirements

- Pi Coding Agent
- `@aefree/pi-subagents` installed in the same Pi environment

## Install

From GitHub:

```bash
pi install git:git@github.com:aefreedman/pi-agents.git
```

Local development install:

```bash
pi install <path-to-pi-agents>
```

Project-local install:

```bash
pi install -l <path-to-pi-agents>
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
