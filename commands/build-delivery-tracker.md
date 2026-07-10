---
name: build-delivery-tracker
description: Build a PubNub-powered real-time order tracking and delivery driver app.
---

Build a real-time delivery tracking application using PubNub.

Before writing any code, present a plan covering:
- Channel architecture for driver location streams, order status, and customer notifications
- GPS location publishing frequency and payload design
- Order lifecycle state machine
- Customer-facing tracking page vs driver app vs dispatch dashboard

Then implement:
- GPS location streaming from driver app using publish at configurable intervals
- Customer-facing tracking page subscribing to driver location channel
- Order status updates (accepted → picked up → en route → delivered)
- ETA calculation and geofence triggers using PubNub Functions
- Dispatch coordination channel for fleet management
- Driver presence tracking (online/offline/active delivery)

Use the `write_pubnub_app` MCP tool for architecture best practices.
