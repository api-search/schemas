---
description: Destination schema from Ampersand API
layout: schema
name: Destination
properties_list:
- description: The destination ID.
  name: id
  type: string
- description: User-defined name for the destination
  name: name
  type: string
- description: The type of the destination
  name: type
  type: string
- description: ''
  name: metadata
  type: object
- description: The time the destination was created.
  name: createTime
  type: string
- description: The time the destination was updated.
  name: updateTime
  type: string
provider_name: Ampersand
provider_slug: ampersand
schema_file: json-schema/ampersand-api-destination-schema.json
slug: ampersand-api-destination
source_filename: ampersand-api-destination-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/ampersand/refs/heads/main/json-schema/ampersand-api-destination-schema.json\",\n  \"title\": \"Destination\",\n  \"description\": \"Destination schema from Ampersand API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The destination ID.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"User-defined name for the destination\",\n      \"example\": \"leadConvertedWebhook\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"The type of the destination\",\n      \"example\": \"webhook\"\n    },\n    \"metadata\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"url\": {\n          \"type\": \"string\",\n          \"description\": \"Webhook URL\",\n          \"example\": \"https://webhooks.mailmonkey.com/salesforce-lead-converted\"\
  \n        },\n        \"headers\": {\n          \"$ref\": \"#/components/schemas/WebhookHeaders\"\n        },\n        \"streamName\": {\n          \"type\": \"string\",\n          \"description\": \"The name of the Kinesis stream\",\n          \"example\": \"my-data-stream\"\n        },\n        \"region\": {\n          \"type\": \"string\",\n          \"description\": \"The AWS region for the destination\",\n          \"example\": \"us-east-1\"\n        },\n        \"partitionKeyTemplate\": {\n          \"type\": \"string\",\n          \"description\": \"Template for generating partition keys\",\n          \"example\": \"{{.integration_id}}\"\n        }\n      }\n    },\n    \"createTime\": {\n      \"type\": \"string\",\n      \"description\": \"The time the destination was created.\",\n      \"format\": \"date-time\"\n    },\n    \"updateTime\": {\n      \"type\": \"string\",\n      \"description\": \"The time the destination was updated.\",\n      \"format\": \"date-time\"\n    }\n\
  \  },\n  \"required\": [\n    \"id\",\n    \"name\",\n    \"type\",\n    \"metadata\",\n    \"createTime\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/ampersand/refs/heads/main/json-schema/ampersand-api-destination-schema.json
tags:
- Developer Tools
- Integrations
- Platform
- SaaS
- OAuth
- Data Sync
- Webhooks
title: Destination
---
