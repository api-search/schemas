---
description: Breakdown of Copilot seat counts by status.
layout: schema
name: SeatBreakdown
properties_list:
- description: Total number of Copilot seats.
  name: total
  type: integer
- description: Seats added in the current billing cycle.
  name: added_this_cycle
  type: integer
- description: Seats with pending invitations.
  name: pending_invitation
  type: integer
- description: Seats pending cancellation at end of cycle.
  name: pending_cancellation
  type: integer
- description: Seats active in the current billing cycle.
  name: active_this_cycle
  type: integer
- description: Seats inactive in the current billing cycle.
  name: inactive_this_cycle
  type: integer
provider_name: GitHub Copilot
provider_slug: github-copilot
schema_file: json-schema/github-copilot-seat-breakdown-schema.json
slug: github-copilot-seat-breakdown
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"SeatBreakdown\",\n  \"type\": \"object\",\n  \"description\": \"Breakdown of Copilot seat counts by status.\",\n  \"properties\": {\n    \"total\": {\n      \"type\": \"integer\",\n      \"description\": \"Total number of Copilot seats.\"\n    },\n    \"added_this_cycle\": {\n      \"type\": \"integer\",\n      \"description\": \"Seats added in the current billing cycle.\"\n    },\n    \"pending_invitation\": {\n      \"type\": \"integer\",\n      \"description\": \"Seats with pending invitations.\"\n    },\n    \"pending_cancellation\": {\n      \"type\": \"integer\",\n      \"description\": \"Seats pending cancellation at end of cycle.\"\n    },\n    \"active_this_cycle\": {\n      \"type\": \"integer\",\n      \"description\": \"Seats active in the current billing cycle.\"\n    },\n    \"inactive_this_cycle\": {\n      \"type\": \"integer\",\n      \"description\": \"Seats inactive in the\
  \ current billing cycle.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/github-copilot/refs/heads/main/json-schema/github-copilot-seat-breakdown-schema.json
tags:
- Agents
- AI
- Artificial Intelligence
- Code Generation
- Code Review
- Coding Agent
- Custom Instructions
- Developer Tools
- Extensions
- IDE
- Machine Learning
- MCP
- Metrics
- Model Context Protocol
- Productivity
title: SeatBreakdown
---
