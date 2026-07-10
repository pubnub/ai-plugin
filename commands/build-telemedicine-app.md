---
name: build-telemedicine-app
description: Build a HIPAA-compliant PubNub telemedicine app with secure messaging and virtual waiting rooms.
---

Build a HIPAA-compliant telemedicine application using PubNub.

Before writing any code, present a plan covering:
- HIPAA compliance requirements for realtime messaging (encryption, access control, audit logging)
- Channel architecture for patient-provider sessions and virtual waiting rooms
- Access Manager token strategy for patient/provider role separation
- WebRTC signaling design for video consultations
- Audit logging approach for compliance

Then implement:
- Secure patient-provider messaging with AES-256 encryption
- Access Manager tokens with role-based permissions (patient vs provider)
- Virtual waiting room with queue management using Presence
- WebRTC signaling channel for video consultation setup
- Consent management flow before session start
- Audit log publishing for compliance record-keeping

Use the `write_pubnub_app` MCP tool for security best practices.
Use the `get_sdk_documentation` MCP tool for Access Manager implementation.
