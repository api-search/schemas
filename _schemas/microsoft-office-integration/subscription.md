---
description: An Office 365 Management Activity API subscription to a content type for receiving audit activity data.
layout: schema
name: Subscription
properties_list:
- description: The content type of the subscription.
  name: contentType
  type: string
- description: The status of the subscription.
  name: status
  type: string
- description: The webhook configuration associated with the subscription.
  name: webhook
  type:
  - object
  - 'null'
provider_name: Microsoft Office Integration
provider_slug: microsoft-office-integration
schema_file: json-schema/subscription.json
slug: subscription
source_filename: subscription.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"subscription.json\",\n  \"title\": \"Subscription\",\n  \"description\": \"An Office 365 Management Activity API subscription to a content type for receiving audit activity data.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"contentType\": {\n      \"type\": \"string\",\n      \"description\": \"The content type of the subscription.\",\n      \"enum\": [\n        \"Audit.AzureActiveDirectory\",\n        \"Audit.Exchange\",\n        \"Audit.SharePoint\",\n        \"Audit.General\",\n        \"DLP.All\"\n      ]\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"The status of the subscription.\",\n      \"enum\": [\"enabled\", \"disabled\"]\n    },\n    \"webhook\": {\n      \"type\": [\"object\", \"null\"],\n      \"description\": \"The webhook configuration associated with the subscription.\",\n      \"properties\": {\n        \"status\": {\n          \"\
  type\": \"string\",\n          \"description\": \"The status of the webhook.\",\n          \"enum\": [\"enabled\", \"disabled\", \"expired\"]\n        },\n        \"address\": {\n          \"type\": \"string\",\n          \"format\": \"uri\",\n          \"description\": \"The HTTPS endpoint that receives notifications.\"\n        },\n        \"authId\": {\n          \"type\": \"string\",\n          \"description\": \"String included as Webhook-AuthID header in notifications.\"\n        },\n        \"expiration\": {\n          \"type\": [\"string\", \"null\"],\n          \"format\": \"date-time\",\n          \"description\": \"Datetime after which notifications are no longer sent to the webhook.\"\n        }\n      },\n      \"required\": [\"status\", \"address\"]\n    }\n  },\n  \"required\": [\"contentType\", \"status\"]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-office-integration/refs/heads/main/json-schema/subscription.json
tags:
- Microsoft 365
- Microsoft Office Integration
- Office 365
title: Subscription
---
