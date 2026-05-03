---
description: An integration instance configured in Zluri for syncing data from external applications.
layout: schema
name: Zluri Integration Instance
properties_list:
- description: Unique identifier of the instance.
  name: id
  type: string
- description: Name of the integration instance.
  name: name
  type: string
- description: Current status of the instance.
  name: status
  type: string
- description: Email addresses to receive sync notifications.
  name: notification_emails
  type: array
- description: When the instance was created.
  name: created_at
  type: string
- description: When the instance was last updated.
  name: updated_at
  type: string
provider_name: Zluri
provider_slug: zluri
schema_file: json-schema/instance.json
slug: instance
source_filename: instance.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/zluri/refs/heads/main/json-schema/instance.json\",\n  \"title\": \"Zluri Integration Instance\",\n  \"description\": \"An integration instance configured in Zluri for syncing data from external applications.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier of the instance.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the integration instance.\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Current status of the instance.\",\n      \"enum\": [\"active\", \"inactive\"]\n    },\n    \"notification_emails\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\",\n        \"format\": \"email\"\n      },\n      \"description\": \"Email addresses to receive sync\
  \ notifications.\"\n    },\n    \"created_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"When the instance was created.\"\n    },\n    \"updated_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"When the instance was last updated.\"\n    }\n  },\n  \"required\": [\"id\", \"name\", \"status\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/zluri/refs/heads/main/json-schema/instance.json
tags:
- Access Management
- SaaS Management
title: Zluri Integration Instance
---
