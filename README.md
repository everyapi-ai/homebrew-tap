# Homebrew Tap for EveryAPI

Homebrew formula for the [EveryAPI](https://everyapi.ai) CLI.

## Install

```bash
brew tap everyapi-ai/tap
brew install everyapi        # CLI: route Claude Code / Codex / Gemini CLI through EveryAPI
```

Or in one shot:

```bash
brew install everyapi-ai/tap/everyapi
```

## Available formulas

| Formula  | Description |
|----------|-------------|
| `everyapi` | EveryAPI CLI. One command (`everyapi use claude / codex / gemini`) configures any supported third-party CLI to route through EveryAPI. The MCP server ships in the same binary as the `everyapi mcp` subcommand. |

Pure-Go binary, no runtime dependencies; one bottle per supported platform (`linux_amd64` / `linux_arm64` / `darwin_amd64` / `darwin_arm64`; Windows is published as a `.zip` on the [release page](https://github.com/everyapi-ai/everyapi-ai/releases) but not as a Homebrew bottle).

## Source

Canonical source code lives in the monorepo: [`everyapi-ai/everyapi/clients/cli`](https://github.com/everyapi-ai/everyapi/tree/main/clients/cli). A path-rewritten copy is mirrored to [`everyapi-ai/everyapi-ai`](https://github.com/everyapi-ai/everyapi-ai) so `go install github.com/everyapi-ai/everyapi-ai@latest` works.

This tap is **auto-generated** by the [release workflow](https://github.com/everyapi-ai/everyapi/blob/main/.github/workflows/cli-release.yml) on every `v*` tag — do not edit files in this repository by hand, the next release will overwrite them. Open issues and PRs against the monorepo, not against this tap.

## License

MIT — see [`everyapi-ai/everyapi/clients/cli/LICENSE`](https://github.com/everyapi-ai/everyapi/blob/main/clients/cli/LICENSE) on the source repo.
