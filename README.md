# create-codex

[![npm](https://img.shields.io/npm/v/create-codex)](https://www.npmjs.com/package/create-codex)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)

AGENTS.md is the open standard for AI coding agent instructions, supported across Codex, Cursor, Aider, Jules, Zed, Windsurf, Continue, and 20k+ projects. I wanted one command to drop a well-tuned AGENTS.md into any project, with runtime/framework/package manager auto-detection baked in. So I built this.

AGENTS.md setup that just works. Bootstrap every project with the open standard for AI coding agents. One command, zero dependencies, zero overhead.

## Quick start

```bash
npm create codex
```

## Install

```bash
npm create codex               # npm
pnpm create codex              # pnpm
bun create codex               # bun
yarn create codex              # yarn
```

Flags:

```bash
npm create codex --dry-run     # preview files
npm create codex --help        # all options
```

Shortcuts:

```bash
npx create-codex my-project    # create in specific directory
```

## Programmatic

```bash
npm i create-codex
```

```typescript
import { init } from 'create-codex';

await init('./my-project');
```

## What's in the box

### Universal compatibility

One AGENTS.md file that any agent supporting the standard can read: Codex, Cursor, Aider, Jules, Zed, Windsurf, Continue.

### Auto-detection

- **Runtimes**: Node.js, Python, Rust, Go, Java, C/C++, TypeScript, Bun
- **Frameworks**: React, Next.js, Vue, Angular, Svelte, Express, FastAPI
- **Package managers**: npm, yarn, pnpm, bun, pip, poetry, uv
- **Git**: repository URL, branch, user info

### Safety

- Atomic writes with SHA256 verification
- Timestamped backups of existing files
- Template rendering with conditionals and variable substitution

### Smart AGENTS.md output

- Setup/dev/build/test commands for your stack
- Language-specific conventions
- Step-by-step workflow
- Safety boundaries and operational limits
- Project context: path, git info, environment

## Requirements

- Node.js 20+
- Any AI agent that supports [AGENTS.md](https://agents.md)

## What gets created

```
AGENTS.md
```

## Remove it

```bash
rm AGENTS.md
```

Your original code stays untouched.

## License

MIT
