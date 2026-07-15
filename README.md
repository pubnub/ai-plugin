# PubNub Realtime Development for Cursor

Build production-ready chat, multiplayer games, live events, auctions, delivery tracking, and collaborative apps using natural language — powered by the Hosted PubNub MCP Server and PubNub AI Skills.

## What's Included

| Component | Details |
|-----------|---------|
| **Hosted MCP Server** | 16 tools via `https://mcp.pubnub.com` — pub/sub, presence, history, App Context, Illuminate, Insights, keyset management |
| **22 AI Skills** | Domain-specific knowledge covering every major PubNub feature and vertical use case |
| **8 Slash Commands** | Ready-to-use prompt templates for the most common realtime use cases |
| **Best-Practice Rules** | Always-on guidance: no exposed keys, persistent userId, retry logic, TLS |

## Install

Install from the [Cursor Marketplace](https://cursor.com/marketplace) — search for **PubNub Realtime Development**.

On install:
1. Cursor loads the plugin and connects to `https://mcp.pubnub.com`
2. You'll be prompted to authenticate with your PubNub account via OAuth
3. All 16 MCP tools become available in the Cursor agent
4. Skills activate automatically based on what you're building

## Skills

Skills teach the Cursor agent how to build with PubNub correctly. They activate automatically in **Agent Decides** mode — no slash commands needed.

### Foundational Skills

| Skill | Invoked when you mention... |
|-------|-----------------------------|
| `pubnub-app-developer` | pub/sub, channels, subscribe, publish, realtime |
| `pubnub-chat` | chat, messaging, direct message, group channel |
| `pubnub-presence` | online users, presence, who is connected, occupancy |
| `pubnub-security` | auth, encrypt, Access Manager, tokens, HIPAA |
| `pubnub-app-context` | user metadata, channel metadata, memberships, Objects API |
| `pubnub-scale` | high volume, channel groups, 10K+ users, performance |

### Cross-Cutting Skills

| Skill | Invoked when you mention... |
|-------|-----------------------------|
| `pubnub-reliability` | reconnect, missed messages, retry, offline, idempotent |
| `pubnub-functions` | serverless, webhook, edge function, KVStore, scheduled |
| `pubnub-history` | message history, storage, catch-up, pagination |
| `pubnub-events-and-actions` | webhook, Lambda, Kafka, SQS, EventBridge, S3 |
| `pubnub-observability` | logging, debugging, cost, incident, usage metrics |
| `pubnub-keyset-management` | keys, keysets, environments, dev/prod, key rotation |
| `pubnub-illuminate` | analytics, decisions, business objects, metrics, automation |
| `pubnub-choose-docs-path` | routes intent to the right skill and MCP tool automatically |

### Vertical / Use-Case Skills

| Skill | Invoked when you mention... |
|-------|-----------------------------|
| `pubnub-multiplayer-gaming` | multiplayer, game lobby, state sync, matchmaking, Unity, Unreal |
| `pubnub-live-auctions` | auction, bidding, countdown timer, anti-sniping |
| `pubnub-live-sport-updates` | sports scores, scoreboard, play-by-play, live feed |
| `pubnub-live-stock-quote-updates` | stock quotes, market data, price alerts, watchlist |
| `pubnub-live-betting-casino` | betting, in-play odds, casino, wager, compliance |
| `pubnub-live-voting` | voting, polling, vote tally, live results |
| `pubnub-order-delivery-driver` | delivery tracking, GPS, order status, driver, dispatch |
| `pubnub-telemedicine` | telemedicine, HIPAA, patient, waiting room, WebRTC |

## Slash Commands

Type any of these in the Cursor chat to start a guided build:

| Command | What it builds |
|---------|----------------|
| `/scaffold-pubnub-app` | A new PubNub app tailored to your language and use case |
| `/build-chat-app` | Full chat with messaging, presence, history, and user profiles |
| `/build-multiplayer-game` | Game lobby, state sync, matchmaking, and reconnect handling |
| `/build-live-auction` | Realtime bidding, anti-sniping, presence, and bid history |
| `/build-sports-dashboard` | Live scores, play-by-play feed, and viewer count |
| `/build-delivery-tracker` | GPS streaming, order status pipeline, and customer tracking |
| `/build-telemedicine-app` | HIPAA-compliant chat, virtual waiting room, and WebRTC signaling |
| `/setup-illuminate` | Realtime analytics pipeline, Decisions, and automation |

## Example Prompts

Copy and paste any of these directly into Cursor chat:

```
Build a React multiplayer trivia game with PubNub — include a lobby,
real-time question broadcasting, answer collection, and a live leaderboard.
```

```
Add live auction bidding to my existing app. Include realtime bid updates,
active bidder count, anti-sniping behavior, and server-side bid validation.
```

```
Set up HIPAA-compliant chat for a telemedicine platform — secure messaging
between patients and providers, a virtual waiting room, and an audit log.
```

```
Build a live sports dashboard showing real-time scores and play-by-play
for multiple matches, with catch-up for users who join mid-game.
```

```
Add real-time stock quote streaming to my trading app with price alerts
and a live watchlist showing top movers.
```

```
Build a live voting system for a TV show audience — realtime vote tallying,
duplicate prevention, and a live results leaderboard.
```

## MCP Tools Reference

The PubNub MCP server exposes 16 tools across 5 categories. Full reference at [pubnub.com/docs/ai/available-mcp-tools](https://www.pubnub.com/docs/ai/available-mcp-tools).

| Category | Tools |
|----------|-------|
| Documentation | `get_sdk_documentation`, `get_chat_sdk_documentation`, `how_to`, `write_pubnub_app`, `get_sdk_migration_guide`, `get_general_migration_guide` |
| App & Keyset management | `manage_apps`, `manage_keysets`, `get_usage_metrics` |
| Real-time communication | `send_pubnub_message`, `subscribe_and_receive_pubnub_messages`, `get_pubnub_messages`, `get_pubnub_presence`, `manage_app_context` |
| Illuminate analytics | `manage_illuminate` |
| Insights analytics | `insights` |

## Local Development

To test the plugin locally before it's live on the Marketplace:

```bash
ln -s /path/to/pubnub-realtime-development ~/.cursor/plugins/local/pubnub-realtime-development
```

Then reload Cursor (`Cmd+Shift+P` → **Developer: Reload Window**) and verify the plugin loads under **Customize**.

## Resources

- [PubNub Documentation](https://www.pubnub.com/docs)
- [PubNub MCP Server](https://www.pubnub.com/docs/ai/pubnub-mcp-server)
- [Available MCP Tools](https://www.pubnub.com/docs/ai/available-mcp-tools)
- [PubNub Skills on GitHub](https://github.com/pubnub/skills)
- [PubNub Admin Portal](https://admin.pubnub.com)
