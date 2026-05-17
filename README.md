# Homebrew Tap for Relaya

Homebrew formulas for the [Relaya](https://relaya.pro) CLI and MCP server.

> ⏳ **Pending first release.** Formula files will land here once the first `cli-v*` tag is pushed on the [source repo](https://github.com/relaya-ai/relaya). Until then `brew install` won't find anything — see the install section below for what will work once the formulas appear.

## Install (once formulas land)

```bash
brew tap relaya-ai/tap
brew install relaya         # CLI: route Claude Code / Codex / Gemini CLI through Relaya
brew install relaya-mcp     # MCP server: expose Relaya as Model Context Protocol tools
```

## Available formulas (planned)

| Formula | Description |
|---|---|
| `relaya` | Buyer onboarding CLI for the Relaya AI gateway. One command (`relaya use claude / codex / gemini`) configures any supported third-party CLI to route through Relaya. |
| `relaya-mcp` | Model Context Protocol server. Lets Claude Code / Cursor / any MCP client invoke Relaya operations (status, top-up, seller channel management) without opening a terminal. |

Both are pure-Go binaries, no runtime dependencies; one bottle per supported platform (linux_amd64 / linux_arm64 / darwin_amd64 / darwin_arm64).

## Source

Canonical source code lives in the main monorepo: [`relaya-ai/relaya/clients/cli`](https://github.com/relaya-ai/relaya/tree/main/clients/cli).

This tap is **auto-generated** by the [release workflow](https://github.com/relaya-ai/relaya/blob/main/.github/workflows/cli-release.yml) on every `cli-v*` tag — do not edit files in this repository by hand, the next release will overwrite them. Open issues and PRs against the main repo, not against this tap.

## License

MIT — see [`relaya-ai/relaya/clients/cli/LICENSE`](https://github.com/relaya-ai/relaya/blob/main/clients/cli/LICENSE) on the source repo.
