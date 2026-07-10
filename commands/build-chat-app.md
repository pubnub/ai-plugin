---
name: build-chat-app
description: Build a PubNub-powered chat application with messaging, presence, and user management.
---

Build a chat application using PubNub.

Before writing any code, present a plan covering:
- Channel architecture (direct messages, group channels, public rooms)
- Message schema and data model
- Presence strategy for online/offline indicators and typing indicators
- User metadata approach using App Context
- History and offline catch-up for users who reconnect

Then implement:
- Real-time messaging with publish/subscribe
- Typing indicators using PubNub signals
- Online/offline presence indicators
- Message history with pagination
- User profiles using App Context (Objects API)
- Read receipts using Message Actions

Use the `get_chat_sdk_documentation` MCP tool for Chat SDK features.
Use the `write_pubnub_app` MCP tool for architecture best practices.
