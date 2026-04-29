---
description: Represents a call in Teams.
layout: schema
name: Call
properties_list:
- description: Unique identifier for the call.
  name: id
  type: string
- description: Current call state.
  name: state
  type: string
- description: Direction of the call.
  name: direction
  type: string
- description: Subject of the call.
  name: subject
  type: string
- description: Callback URL for call notifications.
  name: callbackUri
  type: string
- description: Requested communication modalities.
  name: requestedModalities
  type: array
provider_name: Microsoft Teams
provider_slug: microsoft-teams
schema_file: json-schema/teams-graph-api-call-schema.json
slug: teams-graph-api-call
source_filename: teams-graph-api-call-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/microsoft-teams/refs/heads/main/json-schema/teams-graph-api-call-schema.json\",\n  \"title\": \"Call\",\n  \"description\": \"Represents a call in Teams.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": { \"type\": \"string\", \"description\": \"Unique identifier for the call.\" },\n    \"state\": { \"type\": \"string\", \"enum\": [\"incoming\", \"establishing\", \"ringing\", \"established\", \"hold\", \"transferring\", \"transferAccepted\", \"redirecting\", \"terminating\", \"terminated\"], \"description\": \"Current call state.\" },\n    \"direction\": { \"type\": \"string\", \"enum\": [\"incoming\", \"outgoing\"], \"description\": \"Direction of the call.\" },\n    \"subject\": { \"type\": \"string\", \"description\": \"Subject of the call.\" },\n    \"callbackUri\": { \"type\": \"string\", \"format\": \"uri\", \"description\": \"\
  Callback URL for call notifications.\" },\n    \"requestedModalities\": { \"type\": \"array\", \"items\": { \"type\": \"string\", \"enum\": [\"audio\", \"video\", \"videoBasedScreenSharing\"] }, \"description\": \"Requested communication modalities.\" }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-teams/refs/heads/main/json-schema/teams-graph-api-call-schema.json
tags:
- Chat
- Collaboration
- Communication
- Microsoft 365
- Productivity
- Video Conferencing
title: Call
---
