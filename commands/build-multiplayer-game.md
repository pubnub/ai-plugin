---
name: build-multiplayer-game
description: Build a PubNub-powered multiplayer game with lobbies, state sync, and presence.
---

Build a multiplayer game using PubNub.

Before writing any code, present a plan covering:
- Channel architecture for lobbies, game rooms, and game state
- Game state synchronization strategy (full state vs delta updates)
- Presence for tracking connected players
- Matchmaking approach
- Handling player disconnects and reconnects mid-game

Then implement:
- Game lobby with player list using Presence (HereNow)
- Real-time game state sync using publish/subscribe with delta updates
- Player join/leave handling with Presence events
- Reconnection logic with state catch-up
- Anti-cheat guidance (server-side validation pattern)

Use the `how_to` MCP tool with Unity or Unreal guides if relevant to the user's platform.
Use the `write_pubnub_app` MCP tool for architecture best practices.
