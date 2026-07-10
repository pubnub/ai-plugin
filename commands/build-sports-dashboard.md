---
name: build-sports-dashboard
description: Build a PubNub-powered live sports scores and play-by-play dashboard.
---

Build a live sports dashboard using PubNub.

Before writing any code, present a plan covering:
- Channel architecture for scores, play-by-play events, and match metadata
- Data publishing strategy (score updates vs full game state)
- Presence for tracking active viewers
- History for users who connect mid-game

Then implement:
- Live score ticker with realtime pub/sub updates
- Play-by-play event feed with message history
- Multi-sport channel hierarchy (e.g. `sport.<sportId>.match.<matchId>`)
- Viewer count using Presence occupancy
- Catch-up for late-joining viewers using Message Persistence
- Fan engagement features (reactions, polls)

Use the `get_sdk_documentation` MCP tool for the user's chosen platform.
Use the `write_pubnub_app` MCP tool for architecture best practices.
