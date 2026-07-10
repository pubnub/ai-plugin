---
name: scaffold-pubnub-app
description: Scaffold a new PubNub realtime application with best-practice architecture.
---

Scaffold a new PubNub realtime application.

Before writing any code:
1. Ask the user for: programming language or framework, primary use case (chat, gaming, live data, etc.), and expected scale (rough number of concurrent users).
2. Use the `write_pubnub_app` MCP tool to load PubNub best practices for architecture, security, and channel design.
3. Present a plan covering: channel naming strategy, SDK initialization pattern, publish/subscribe flow, presence requirements, and security approach.

Then generate:
- SDK initialization with persistent `userId`
- Channel subscription with message listener
- Publish function with error handling
- Connection status handler with reconnect logic
- Environment variable setup for publish/subscribe keys (never hardcoded)

Use the `get_sdk_documentation` MCP tool for the user's chosen language.
