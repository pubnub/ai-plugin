---
name: setup-illuminate
description: Set up PubNub Illuminate for realtime analytics, decisions, and automation pipelines.
---

Set up PubNub Illuminate for realtime analytics and event-driven automation.

Start by asking:
1. What is the goal? (reward engaged users / detect spam or abuse / alert on operational anomalies / automate live event actions)
2. What data is already flowing through PubNub channels?
3. What action should Illuminate take when a condition is met? (notify via webhook, reward a user, moderate a user, trigger a workflow)

Then use the `manage_illuminate` MCP tool to:
- List existing Business Objects and check if a suitable one already exists
- Create a Business Object that maps message fields to Illuminate dimensions
- Create Metrics (COUNT, SUM, AVG) for the KPIs being measured
- Create a Dashboard for visibility
- Create and activate a Decision with the confirmed conditions and actions
- Publish fake test data using `publish-fake-data` to verify the pipeline fires correctly
- Check the action log to confirm the Decision is firing

Use the `how_to` MCP tool for Illuminate conceptual guides.
