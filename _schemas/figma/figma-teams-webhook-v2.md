---
description: A description of an HTTP webhook (from Figma back to your application)
layout: schema
name: WebhookV2
properties_list:
- description: The ID of the webhook
  name: id
  type: string
- description: The team id you are subscribed to for updates
  name: team_id
  type: string
- description: The client ID of the OAuth application that registered this webhook, if any
  name: client_id
  type: '[''string'', ''null'']'
- description: The passcode that will be passed back to the webhook endpoint
  name: passcode
  type: string
- description: The endpoint that will be hit when the webhook is triggered
  name: endpoint
  type: string
- description: Optional user-provided description or name for the webhook. This is provided to help make maintaining a number of webhooks more convenient. Max length 140 characters.
  name: description
  type: '[''string'', ''null'']'
provider_name: Figma
provider_slug: figma
schema_file: json-schema/figma-teams-webhook-v2-schema.json
slug: figma-teams-webhook-v2
source_filename: figma-teams-webhook-v2-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"WebhookV2\",\n  \"type\": \"object\",\n  \"description\": \"A description of an HTTP webhook (from Figma back to your application)\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The ID of the webhook\"\n    },\n    \"team_id\": {\n      \"type\": \"string\",\n      \"description\": \"The team id you are subscribed to for updates\"\n    },\n    \"client_id\": {\n      \"type\": \"['string', 'null']\",\n      \"description\": \"The client ID of the OAuth application that registered this webhook, if any\"\n    },\n    \"passcode\": {\n      \"type\": \"string\",\n      \"description\": \"The passcode that will be passed back to the webhook endpoint\"\n    },\n    \"endpoint\": {\n      \"type\": \"string\",\n      \"description\": \"The endpoint that will be hit when the webhook is triggered\"\n    },\n    \"description\": {\n      \"type\": \"['string',\
  \ 'null']\",\n      \"description\": \"Optional user-provided description or name for the webhook. This is provided to help make maintaining a number of webhooks more convenient. Max length 140 characters.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/figma/refs/heads/main/json-schema/figma-teams-webhook-v2-schema.json
tags:
- Collaboration
- Design
- Graphics
- Interfaces
- Prototypes
- Prototyping
- UI/UX
title: WebhookV2
---
