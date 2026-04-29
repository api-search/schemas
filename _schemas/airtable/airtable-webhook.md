---
description: An Airtable webhook subscription that monitors a base for changes and sends notifications to a specified URL. Webhooks expire after 7 days and must be periodically refreshed.
layout: schema
name: Airtable Webhook
properties_list:
- description: The unique identifier for the webhook.
  name: id
  type: string
- description: The type of webhook (e.g., client).
  name: type
  type: string
- description: Whether the webhook is currently active and will process events.
  name: isHookEnabled
  type: boolean
- description: The URL that receives POST notifications when monitored changes occur.
  name: notificationUrl
  type:
  - string
  - 'null'
- description: The cursor position indicating the next unread payload. Used when polling for payloads.
  name: cursorForNextPayload
  type: integer
- description: Whether HTTP notifications are currently being sent to the notification URL.
  name: areNotificationsEnabled
  type: boolean
- description: The time when the webhook was created.
  name: createdTime
  type: string
- description: The time when the webhook will expire if not refreshed. Webhooks expire 7 days after creation or last refresh.
  name: expirationTime
  type: string
- description: The specification defining which changes the webhook monitors, including data types, field filters, and source options.
  name: specification
  type: object
provider_name: Airtable
provider_slug: airtable
schema_file: json-schema/airtable-webhook-schema.json
slug: airtable-webhook
source_filename: airtable-webhook-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://schemas.airtable.com/webhook.json\",\n  \"title\": \"Airtable Webhook\",\n  \"description\": \"An Airtable webhook subscription that monitors a base for changes and sends notifications to a specified URL. Webhooks expire after 7 days and must be periodically refreshed.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier for the webhook.\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"The type of webhook (e.g., client).\"\n    },\n    \"isHookEnabled\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the webhook is currently active and will process events.\"\n    },\n    \"notificationUrl\": {\n      \"type\": [\"string\", \"null\"],\n      \"format\": \"uri\",\n      \"description\": \"The URL that receives POST notifications when monitored changes\
  \ occur.\"\n    },\n    \"cursorForNextPayload\": {\n      \"type\": \"integer\",\n      \"description\": \"The cursor position indicating the next unread payload. Used when polling for payloads.\"\n    },\n    \"areNotificationsEnabled\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether HTTP notifications are currently being sent to the notification URL.\"\n    },\n    \"createdTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The time when the webhook was created.\"\n    },\n    \"expirationTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The time when the webhook will expire if not refreshed. Webhooks expire 7 days after creation or last refresh.\"\n    },\n    \"specification\": {\n      \"type\": \"object\",\n      \"description\": \"The specification defining which changes the webhook monitors, including data types, field filters, and source options.\",\n      \"properties\"\
  : {\n        \"options\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"filters\": {\n              \"type\": \"object\",\n              \"properties\": {\n                \"dataTypes\": {\n                  \"type\": \"array\",\n                  \"description\": \"The types of data changes to monitor.\",\n                  \"items\": {\n                    \"type\": \"string\",\n                    \"enum\": [\"tableData\", \"tableFields\", \"tableMetadata\"]\n                  }\n                },\n                \"recordChangeScope\": {\n                  \"type\": \"string\",\n                  \"description\": \"The scope of record changes to monitor.\"\n                },\n                \"watchDataInFieldIds\": {\n                  \"type\": \"array\",\n                  \"description\": \"Specific field IDs to watch for data changes.\",\n                  \"items\": {\n                    \"type\": \"string\"\n                  }\n         \
  \       },\n                \"watchSchemasOfFieldIds\": {\n                  \"type\": \"array\",\n                  \"description\": \"Specific field IDs to watch for schema changes.\",\n                  \"items\": {\n                    \"type\": \"string\"\n                  }\n                }\n              }\n            }\n          }\n        }\n      }\n    }\n  },\n  \"required\": [\"id\", \"type\"],\n  \"additionalProperties\": false\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/airtable/refs/heads/main/json-schema/airtable-webhook-schema.json
tags:
- Applications
- Collaboration
- Data
- Databases
- Low-Code
- Productivity
- Spreadsheets
title: Airtable Webhook
---
