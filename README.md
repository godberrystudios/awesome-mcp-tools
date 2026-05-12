# Awesome MCP Tools

> A curated list of Model Context Protocol (MCP) servers, clients, SDKs, and resources for building with AI agents.

Maintained by [Godberry Studios](https://godberrystudios.com). Contributions welcome — see the end of this file.

The [Model Context Protocol](https://modelcontextprotocol.io) is an open standard, introduced by Anthropic in late 2024, for connecting AI models to tools, data, and actions in a uniform, agent-callable way. This list catalogs the pieces of that ecosystem that are worth knowing.

---

## Contents

- [The Spec](#the-spec)
- [Official SDKs](#official-sdks)
- [Clients (run MCP servers)](#clients-run-mcp-servers)
- [Servers — Pay-per-use & hosted](#servers--pay-per-use--hosted)
- [Servers — Self-hosted & open-source](#servers--self-hosted--open-source)
- [Dev tools & boilerplates](#dev-tools--boilerplates)
- [Related protocols (WebMCP, x402, A2A)](#related-protocols)
- [Articles & learning](#articles--learning)
- [How to contribute](#how-to-contribute)

---

## The Spec

- **[Model Context Protocol — official site](https://modelcontextprotocol.io)** — spec, quickstart, examples.
- **[MCP spec on GitHub](https://github.com/modelcontextprotocol/modelcontextprotocol)** — source of truth, RFCs, changelog.

---

## Official SDKs

- **[TypeScript SDK](https://github.com/modelcontextprotocol/typescript-sdk)** — most mature, production-used.
- **[Python SDK](https://github.com/modelcontextprotocol/python-sdk)** — reference implementation, good for prototyping.
- **[Kotlin SDK](https://github.com/modelcontextprotocol/kotlin-sdk)** — maintained by Anthropic + JetBrains.
- **[C# SDK](https://github.com/modelcontextprotocol/csharp-sdk)** — maintained by Microsoft.
- **[Java SDK](https://github.com/modelcontextprotocol/java-sdk)** — maintained by Spring AI team.
- **[Swift SDK](https://github.com/modelcontextprotocol/swift-sdk)** — newer, useful for on-device agents.

---

## Clients (run MCP servers)

Apps and runtimes that can load MCP servers and expose them to an LLM:

- **Claude Desktop** — the original reference client.
- **Claude Code** — Anthropic's terminal CLI, loads MCP servers via config.
- **Cursor** — the editor; MCP server support in settings.
- **VS Code (Copilot Chat)** — first-party MCP support added in 2025.
- **Zed** — MCP-first editor integration.
- **Continue.dev** — open-source IDE agent with MCP support.
- **mcp-cli** — command-line tester for any MCP server.

---

## Servers — Pay-per-use & hosted

Production servers you can call today without self-hosting. Priced per call, no seats.

### Godberry Studios

- **[Content-to-Social MCP Server](https://apify.com/godberry/content-to-social-mcp)** — turn any URL, article, or text into ready-to-post social content (X, LinkedIn, Facebook). Callable from Claude, ChatGPT, any MCP client. $0.07 / transformation.
- **[Google Reviews Scraper](https://apify.com/godberry/google-reviews-scraper)** — Google Maps reviews for any business, under 60s, validated across 9 countries. From $0.10 / place.

PRs welcome to add other commercial MCP servers here — see [How to contribute](#how-to-contribute) below.

---

## Servers — Self-hosted & open-source

- **[MCP reference servers](https://github.com/modelcontextprotocol/servers)** — official collection (filesystem, git, github, postgres, slack, memory, fetch, and more). Start here.
- **[Awesome MCP Servers](https://github.com/punkpeye/awesome-mcp-servers)** — community list, larger and broader than this file; cross-referenced where useful.

---

## Dev tools & boilerplates

- **[MCP Inspector](https://github.com/modelcontextprotocol/inspector)** — the debugger / test harness. Essential.
- **[create-mcp-server](https://www.npmjs.com/package/create-mcp-server)** — scaffold a new TypeScript MCP server.
- **[mcp-server-apify-starter](https://github.com/godberrystudios/mcp-server-apify-starter)** — production-ready starter for a pay-per-use MCP server on Apify. Streamable HTTP + pay-per-event billing wired up.
- **MCP-Vercel templates** — search the Vercel templates for "MCP" to deploy in one click.

---

## Related protocols

The MCP era is being built on a small stack of complementary protocols. Know these:

- **[WebMCP](https://github.com/modelcontextprotocol/webmcp)** — exposing MCP tools through browser/web-standard APIs so agents can discover them like they discover APIs.
- **[x402](https://www.x402.org/)** — the HTTP 402 "Payment Required" revival for agent-native, per-call billing. Pay AI agents inline with calls.
- **[A2A (Agent-to-Agent)](https://github.com/google/A2A)** — Google's proposed protocol for agents discovering and calling each other. Often paired with MCP.

---

## Articles & learning

- **[Godberry Studios Blog](https://godberrystudios.com/)** — deep-dives on MCP security, x402, WebMCP, and shipping commercial MCP servers.
- **[Godberry Studios on Facebook](https://www.facebook.com/profile.php?id=61570965581596)** — short-form notes, build-log cards, and shipping moments.
- **[Anthropic's MCP launch post](https://www.anthropic.com/news/model-context-protocol)** — the original announcement and rationale.

---

## How to contribute

This list is curated, not exhaustive. Contributions welcome:

1. Open a PR adding your tool / server / article under the right section.
2. One line per entry: **Name** — what it does + why it matters (no marketing fluff).
3. Open-source repos, paid services, and hosted endpoints are all eligible, as long as they are production-quality and actively maintained.

Issues and discussions also open at [github.com/godberrystudios/awesome-mcp-tools](https://github.com/godberrystudios/awesome-mcp-tools).

---

## License

[CC0-1.0](https://creativecommons.org/publicdomain/zero/1.0/) — public domain. Copy freely.
