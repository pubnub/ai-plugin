# PubNub Realtime Development

Build production-ready chat, multiplayer games, live events, auctions,
delivery tracking, and collaborative apps using natural language. This plugin
packages PubNub AI Skills, guided commands, and the hosted PubNub MCP server
for AI agents.

## What's Included

| Component | Details |
| --- | --- |
| **Hosted MCP server** | 16 tools through the [PubNub MCP server](https://mcp.pubnub.com) for documentation, messaging, presence, history, App Context, Illuminate, Insights, and keyset management |
| **Skills** | Domain-specific guidance covering PubNub platform features and realtime use cases |
| **Commands** | Guided workflows for common realtime application types |
| **Cursor rules** | Cursor-specific guidance for secure, reliable PubNub implementations |

## Install

### Claude Code

Add the PubNub marketplace and install the plugin:

```text
/plugin marketplace add pubnub/ai-plugin
/plugin install pubnub-realtime-development@pubnub
```

The skills and commands load when Claude Code starts a new session. Use `/mcp`
to check the PubNub server connection and complete OAuth authentication when
prompted.

To test a local checkout without installing it:

```bash
claude --plugin-dir .
```

### Claude.ai and Cowork

After the plugin is published in Anthropic's directory, add it from
**Customize > Plugins**. Connect the bundled PubNub connector from the
plugin's **Connectors** tab and sign in with your PubNub account.

For development testing, create a ZIP of this repository and select
**Customize > Plugins > Add > Upload plugin**.

### Cursor

Install from the [Cursor Marketplace](https://cursor.com/marketplace) and
search for **PubNub Realtime Development**.

After installation:

1. Cursor connects to the [PubNub MCP server](https://mcp.pubnub.com).
2. Sign in with your PubNub account through OAuth.
3. The PubNub MCP tools become available to the agent.
4. Skills activate automatically when your request matches their purpose.

## Skills

Skills teach AI agents how to design and implement PubNub features.
The agent selects the relevant skill from your request and loads its detailed
instructions and references only when needed.

### Foundational Skills

| Skill | Use it for |
| --- | --- |
| `pubnub-app-developer` | Pub/sub, channels, subscriptions, publishing, and SDK setup |
| `pubnub-chat` | Direct messages, group chat, typing indicators, and reactions |
| `pubnub-presence` | Online state, occupancy, and connection events |
| `pubnub-security` | Access Manager, tokens, encryption, and compliance |
| `pubnub-app-context` | User, channel, and membership metadata |
| `pubnub-scale` | High-volume applications, channel groups, and performance |

### Cross-Cutting Skills

| Skill | Use it for |
| --- | --- |
| `pubnub-reliability` | Reconnects, retries, deduplication, and offline behavior |
| `pubnub-functions` | Serverless logic, webhooks, transformations, and scheduled work |
| `pubnub-history` | Message persistence, pagination, and reconnect catch-up |
| `pubnub-events-and-actions` | Webhook, Lambda, Kafka, SQS, EventBridge, and S3 integrations |
| `pubnub-observability` | Logging, testing, usage, cost, and incident response |
| `pubnub-keyset-management` | Applications, keysets, environments, and key rotation |
| `pubnub-illuminate` | Analytics, business objects, metrics, decisions, and automation |
| `pubnub-choose-docs-path` | Routing a request to the correct skill, documentation, and MCP tool |

### Vertical and Use-Case Skills

| Skill | Use it for |
| --- | --- |
| `pubnub-multiplayer-gaming` | Lobbies, matchmaking, game state, and player reconnects |
| `pubnub-live-auctions` | Bidding, countdowns, anti-sniping, and bid history |
| `pubnub-live-sport-updates` | Scores, play-by-play, scoreboards, and fan engagement |
| `pubnub-live-stock-quote-updates` | Market data, watchlists, alerts, and ticker displays |
| `pubnub-live-betting-casino` | In-play odds, wagers, game state, and compliance |
| `pubnub-live-voting` | Polling, vote tallying, duplicate prevention, and results |
| `pubnub-order-delivery-driver` | GPS tracking, order status, dispatch, and delivery updates |
| `pubnub-telemedicine` | Secure messaging, waiting rooms, WebRTC signaling, and audit logs |

## Commands

In Cursor, invoke commands by their file name, such as `/build-chat-app`.
In Claude Code and Cowork, use the plugin-qualified form, such as
`/pubnub-realtime-development:build-chat-app`. Claude.ai can also select a
command automatically when a request matches its description.

| Command | What it builds |
| --- | --- |
| `scaffold-pubnub-app` | A PubNub application tailored to a language and use case |
| `build-chat-app` | Chat with messaging, presence, history, and user profiles |
| `build-multiplayer-game` | A lobby, state synchronization, matchmaking, and reconnect handling |
| `build-live-auction` | Realtime bidding, anti-sniping, presence, and bid history |
| `build-sports-dashboard` | Live scores, play-by-play, and viewer presence |
| `build-delivery-tracker` | GPS streaming, order status, dispatch, and customer tracking |
| `build-telemedicine-app` | Secure chat, a virtual waiting room, and WebRTC signaling |
| `setup-illuminate` | Realtime analytics, decisions, and automation |

## Example Prompts

```text
Build a React multiplayer trivia game with PubNub. Include a lobby,
realtime question broadcasting, answer collection, and a live leaderboard.
```

```text
Add live auction bidding to my application. Include realtime bid updates,
active bidder count, anti-sniping behavior, and server-side bid validation.
```

```text
Set up secure chat for a telemedicine platform with patient-provider
messaging, a virtual waiting room, and an audit log.
```

```text
Build a live sports dashboard showing realtime scores and play-by-play for
multiple matches, with catch-up for users who join mid-game.
```

## MCP Connector

The plugin references the hosted [PubNub MCP server](https://mcp.pubnub.com).
The connector uses OAuth to access PubNub resources on your behalf. Do not add
publish, subscribe, secret, or access tokens to the plugin files.

The available MCP tools cover:

- PubNub SDK and Chat SDK documentation
- Application and keyset management
- Message publishing, subscription, and history
- Presence and App Context
- Illuminate and Insights

See the [available MCP tools](https://www.pubnub.com/docs/ai/available-mcp-tools)
for the current tool reference.

## Data

The static plugin files do not collect or store user data. When you connect
the PubNub MCP server and invoke a tool, the AI agent sends the information
required for that request to `mcp.pubnub.com`. Depending on the tool, this can
include your prompt, PubNub account or keyset identifiers, channel names,
message content, metadata, and tool parameters.

## Development and Validation

Validate the plugin structure with Claude Code:

```bash
claude plugin validate .
```

Load the working copy in Claude Code:

```bash
claude --plugin-dir .
```

The Claude and Cursor manifests share the root `skills/`, `commands/`, assets,
and `mcp.json` files.

## Resources

- [PubNub Documentation](https://www.pubnub.com/docs)
- [PubNub MCP Server](https://www.pubnub.com/docs/ai/pubnub-mcp-server)
- [Available MCP Tools](https://www.pubnub.com/docs/ai/available-mcp-tools)
- [PubNub Skills on GitHub](https://github.com/pubnub/skills)
- [PubNub Admin Portal](https://admin.pubnub.com)
- [Claude Plugin Structure and Testing](https://claude.com/docs/plugins/build)

## License

This project is licensed under the terms in [LICENSE](LICENSE).
