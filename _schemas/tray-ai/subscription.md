---
description: A trigger subscription that receives real-time data from a third-party service via a Tray.ai trigger.
layout: schema
name: Tray.ai Trigger Subscription
properties_list:
- description: Unique subscription identifier
  name: id
  type: string
- description: The trigger operation name
  name: triggerName
  type: string
- description: The connector associated with the trigger
  name: connectorName
  type: string
- description: The version of the connector
  name: connectorVersion
  type: string
- description: The authentication ID used by this subscription
  name: authId
  type: string
- description: Current subscription status
  name: status
  type: string
- description: Input configuration for the subscription
  name: input
  type: object
- description: Timestamp when the subscription was created
  name: createdAt
  type: string
provider_name: Tray.ai
provider_slug: tray-ai
schema_file: json-schema/subscription.json
slug: subscription
source_filename: subscription.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/tray-ai/refs/heads/main/json-schema/subscription.json\",\n  \"title\": \"Tray.ai Trigger Subscription\",\n  \"description\": \"A trigger subscription that receives real-time data from a third-party service via a Tray.ai trigger.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique subscription identifier\"\n    },\n    \"triggerName\": {\n      \"type\": \"string\",\n      \"description\": \"The trigger operation name\"\n    },\n    \"connectorName\": {\n      \"type\": \"string\",\n      \"description\": \"The connector associated with the trigger\"\n    },\n    \"connectorVersion\": {\n      \"type\": \"string\",\n      \"description\": \"The version of the connector\"\n    },\n    \"authId\": {\n      \"type\": \"string\",\n      \"description\": \"The authentication ID\
  \ used by this subscription\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Current subscription status\"\n    },\n    \"input\": {\n      \"type\": \"object\",\n      \"description\": \"Input configuration for the subscription\"\n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the subscription was created\"\n    }\n  },\n  \"required\": [\"id\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/tray-ai/refs/heads/main/json-schema/subscription.json
tags:
- Automation
- Integration
- iPaaS
title: Tray.ai Trigger Subscription
---
