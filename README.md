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

Pure-Go binary, no runtime dependencies; one bottle per supported platform (`linux_amd64` / `linux_arm64` / `darwin_amd64` / `darwin_arm64`). Windows is published as a `.zip` on the [release page](https://github.com/everyapi-ai/everyapi-ai/releases) but not as a Homebrew bottle.

## Source & go install

Public source mirror: [`everyapi-ai/everyapi-ai`](https://github.com/everyapi-ai/everyapi-ai). All Homebrew bottles, `go install` targets and release artifacts (with cosign signatures) live there.

```bash
go install github.com/everyapi-ai/everyapi-ai@latest
```

This tap is **auto-generated** on every release — do not edit files in this repository by hand, the next release will overwrite them. Open CLI issues at <https://github.com/everyapi-ai/everyapi-ai/issues>.

## License

MIT — see [`LICENSE`](https://github.com/everyapi-ai/everyapi-ai/blob/main/LICENSE) on the source mirror.
