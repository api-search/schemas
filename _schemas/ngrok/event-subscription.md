---
description: An Event Subscription defines which events trigger notifications and where those notifications are sent.
layout: schema
name: ngrok Event Subscription
properties_list:
- description: Unique identifier for the event subscription.
  name: id
  type: string
- description: URI of the event subscription API resource.
  name: uri
  type: string
- description: Timestamp when the subscription was created.
  name: created_at
  type: string
- description: Arbitrary user-defined metadata.
  name: metadata
  type: string
- description: Human-readable description.
  name: description
  type: string
- description: The event sources that trigger this subscription.
  name: sources
  type: array
- description: References to event destinations where notifications are sent.
  name: destinations
  type: array
provider_name: ngrok
provider_slug: ngrok
schema_file: json-schema/event-subscription.json
slug: event-subscription
source_filename: event-subscription.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-evangelist/ngrok/blob/main/json-schema/event-subscription.json\",\n  \"title\": \"ngrok Event Subscription\",\n  \"description\": \"An Event Subscription defines which events trigger notifications and where those notifications are sent.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the event subscription.\"\n    },\n    \"uri\": {\n      \"type\": \"string\",\n      \"description\": \"URI of the event subscription API resource.\"\n    },\n    \"created_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the subscription was created.\"\n    },\n    \"metadata\": {\n      \"type\": \"string\",\n      \"description\": \"Arbitrary user-defined metadata.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n     \
  \ \"description\": \"Human-readable description.\"\n    },\n    \"sources\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"type\": {\n            \"type\": \"string\",\n            \"description\": \"The type of event source.\"\n          },\n          \"uri\": {\n            \"type\": \"string\",\n            \"description\": \"URI of the event source.\"\n          }\n        }\n      },\n      \"description\": \"The event sources that trigger this subscription.\"\n    },\n    \"destinations\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"id\": {\n            \"type\": \"string\"\n          },\n          \"uri\": {\n            \"type\": \"string\"\n          }\n        }\n      },\n      \"description\": \"References to event destinations where notifications are sent.\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/ngrok/refs/heads/main/json-schema/event-subscription.json
tags:
- AI Gateway
- API Gateway
- Compute
- Developer Tools
- Gateways
- Ingress
- Platform
- Proxies
- Servers
- Tunnels
title: ngrok Event Subscription
---
