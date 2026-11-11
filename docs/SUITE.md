# The local-first developer toolkit

Four small tools, one workflow. Each one solves a narrow problem and can be used alone. Together they cover the path from "my repo is too big for the model" to "I can verify what the vendor just sent me." The `kodyaz` umbrella is the in-progress fifth entry point.

```text
┌──────────────────────────────────────────────────────────────┐
│                        kodyaz (umbrella)                     │
│              one CLI · one MCP server · one config           │
├───────────────┬───────────────┬───────────────┬──────────────┤
│    ctxpack    │  envsentinel  │   hookyard    │   svgforge   │
│  pack a repo  │ validate env  │ inspect hooks │ render SVGs  │
│  for an LLM   │ find secrets  │ verify + replay│ locally     │
└───────────────┴───────────────┴───────────────┴──────────────┘
```

## Why these four belong together

| Stage | Tool | Question it answers |
| --- | --- | --- |
| Context | `ctxpack` | "How do I give an AI enough code without leaking secrets or blowing the budget?" |
| Configuration | `envsentinel` | "Is my `.env` valid, complete, and free of leaked keys?" |
| Integration | `hookyard` | "What did the vendor actually send, and is the signature valid?" |
| Presentation | `svgforge` | "How do I make the README look good without a render service?" |

## The shared contract

Every tool follows the same rules:

1. **No network by default.** Network access is explicit, documented, and opt-in.
2. **Files in, files out.** No proprietary database, no hidden state.
3. **Exit codes are meaningful.** `0` success, `1` user error, `2` bad configuration. CI can depend on them.
4. **MCP where it helps.** `ctxpack`, `envsentinel`, and `hookyard` expose tools to AI agents; `svgforge` stays a pure generator.
5. **Apache-2.0.** One license for the whole suite. GPL-3.0 only where an upstream requires it.
6. **One page of docs per feature.** If a flag needs a paragraph, the flag is wrong.

## Roadmap

- [x] Independent, installable packages
- [x] MCP servers for context, env, and webhook tools
- [x] Published npm packages for `ctxpack`, `envsentinel`, `svgforge`
- [ ] `hookyard` on PyPI
- [ ] `kodyaz` umbrella CLI
- [ ] Single MCP server exposing all tools
- [ ] Shared config file (`kodyaz.toml`)
- [ ] Reproducible demo repository

## What this is not

It is not a platform, a SaaS, or a dashboard. The tools are deliberately boring: they read files, do one thing, and exit. That is the point.
