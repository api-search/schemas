---
description: Topic schema from Ampersand API
layout: schema
name: Topic
properties_list:
- description: The topic ID.
  name: id
  type: string
- description: The name of the topic. Must contain only letters, numbers, and dashes.
  name: name
  type: string
- description: The Ampersand project ID.
  name: projectId
  type: string
- description: The time when the topic was created.
  name: createTime
  type: string
- description: The time when the topic was last updated.
  name: updateTime
  type: string
provider_name: Ampersand
provider_slug: ampersand
schema_file: json-schema/ampersand-api-topic-schema.json
slug: ampersand-api-topic
source_filename: ampersand-api-topic-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/ampersand/refs/heads/main/json-schema/ampersand-api-topic-schema.json\",\n  \"title\": \"Topic\",\n  \"description\": \"Topic schema from Ampersand API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The topic ID.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the topic. Must contain only letters, numbers, and dashes.\",\n      \"example\": \"system-alerts\",\n      \"maxLength\": 64\n    },\n    \"projectId\": {\n      \"type\": \"string\",\n      \"description\": \"The Ampersand project ID.\"\n    },\n    \"createTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The time when the topic was created.\"\n    },\n    \"updateTime\": {\n      \"type\": \"string\",\n      \"format\": \"\
  date-time\",\n      \"description\": \"The time when the topic was last updated.\"\n    }\n  },\n  \"required\": [\n    \"id\",\n    \"name\",\n    \"projectId\",\n    \"createTime\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/ampersand/refs/heads/main/json-schema/ampersand-api-topic-schema.json
tags:
- Developer Tools
- Integrations
- Platform
- SaaS
- OAuth
- Data Sync
- Webhooks
title: Topic
---
