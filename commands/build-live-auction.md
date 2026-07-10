---
name: build-live-auction
description: Build a PubNub-powered live auction app with realtime bidding and anti-sniping.
---

Build a live auction application using PubNub.

Before writing any code, present a plan covering:
- Channel architecture for auction rooms and bid updates
- Bid validation strategy (server-side vs client-side)
- Presence for tracking active bidders
- Anti-sniping logic design
- Bid history and audit trail approach

Then implement:
- Realtime bid broadcasts using publish/subscribe
- Active bidder tracking using Presence (HereNow)
- Bid history using Message Persistence
- Anti-sniping behavior: when a bid arrives in the final 10 seconds, extend the auction timer
- Server-side bid validation pattern to prevent client-side manipulation
- Outbid notifications to all participants

Use the `write_pubnub_app` MCP tool for architecture best practices.
