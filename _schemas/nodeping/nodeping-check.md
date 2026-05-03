---
description: Schema for a NodePing monitoring check.
layout: schema
name: NodePing Check
properties_list:
- description: NodePing check identifier
  name: _id
  type: string
- description: Check type (HTTP, DNS, SMTP, PING, SSL, etc.)
  name: type
  type: string
- description: Target URL, host, or address being checked
  name: target
  type: string
- description: Human-readable label
  name: label
  type: string
- description: Run interval in minutes
  name: interval
  type: integer
- description: Whether the check is active
  name: enabled
  type: boolean
- description: Whether results are publicly viewable
  name: public
  type: boolean
- description: Response time threshold
  name: threshold
  type: integer
- description: Sensitivity (consecutive failures before alerting)
  name: sens
  type: integer
- description: Run automatic diagnostics on failure
  name: autodiag
  type: boolean
- description: Home probe location
  name: homeloc
  type: string
- description: Probe regions where the check runs
  name: runlocations
  type: array
- description: Dependency check id
  name: dep
  type: string
- description: Whether notifications are muted
  name: mute
  type: boolean
- description: ''
  name: description
  type: string
- description: ''
  name: tags
  type: array
- description: Notification routing for the check
  name: notifications
  type: array
- description: Current state (1 up, 0 down)
  name: state
  type: integer
- description: ''
  name: uuid
  type: string
- description: Created timestamp (epoch)
  name: created
  type: integer
- description: Modified timestamp (epoch)
  name: modified
  type: integer
provider_name: NodePing
provider_slug: nodeping
schema_file: json-schema/nodeping-check-schema.json
slug: nodeping-check
source_filename: nodeping-check-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/nodeping/refs/heads/main/json-schema/nodeping-check-schema.json\",\n  \"title\": \"NodePing Check\",\n  \"description\": \"Schema for a NodePing monitoring check.\",\n  \"type\": \"object\",\n  \"required\": [\"type\"],\n  \"properties\": {\n    \"_id\": { \"type\": \"string\", \"description\": \"NodePing check identifier\" },\n    \"type\": { \"type\": \"string\", \"description\": \"Check type (HTTP, DNS, SMTP, PING, SSL, etc.)\" },\n    \"target\": { \"type\": \"string\", \"description\": \"Target URL, host, or address being checked\" },\n    \"label\": { \"type\": \"string\", \"description\": \"Human-readable label\" },\n    \"interval\": { \"type\": \"integer\", \"description\": \"Run interval in minutes\" },\n    \"enabled\": { \"type\": \"boolean\", \"description\": \"Whether the check is active\" },\n    \"public\": { \"type\": \"boolean\"\
  , \"description\": \"Whether results are publicly viewable\" },\n    \"threshold\": { \"type\": \"integer\", \"description\": \"Response time threshold\" },\n    \"sens\": { \"type\": \"integer\", \"description\": \"Sensitivity (consecutive failures before alerting)\" },\n    \"autodiag\": { \"type\": \"boolean\", \"description\": \"Run automatic diagnostics on failure\" },\n    \"homeloc\": { \"type\": \"string\", \"description\": \"Home probe location\" },\n    \"runlocations\": {\n      \"type\": \"array\",\n      \"items\": { \"type\": \"string\" },\n      \"description\": \"Probe regions where the check runs\"\n    },\n    \"dep\": { \"type\": \"string\", \"description\": \"Dependency check id\" },\n    \"mute\": { \"type\": \"boolean\", \"description\": \"Whether notifications are muted\" },\n    \"description\": { \"type\": \"string\" },\n    \"tags\": { \"type\": \"array\", \"items\": { \"type\": \"string\" } },\n    \"notifications\": {\n      \"type\": \"array\",\n      \"description\"\
  : \"Notification routing for the check\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"contact\": { \"type\": \"string\" },\n          \"delay\": { \"type\": \"integer\" },\n          \"schedule\": { \"type\": \"string\" }\n        }\n      }\n    },\n    \"state\": { \"type\": \"integer\", \"description\": \"Current state (1 up, 0 down)\" },\n    \"uuid\": { \"type\": \"string\" },\n    \"created\": { \"type\": \"integer\", \"description\": \"Created timestamp (epoch)\" },\n    \"modified\": { \"type\": \"integer\", \"description\": \"Modified timestamp (epoch)\" }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/nodeping/refs/heads/main/json-schema/nodeping-check-schema.json
tags:
- Monitoring
- Uptime
- Notifications
- SaaS
title: NodePing Check
---
