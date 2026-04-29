---
description: ''
layout: schema
name: WebhookSecret
properties_list:
- description: The name of the secret.
  name: name
  type: string
- description: The database which stores the secret.
  name: database_name
  type: string
- description: The schema which stores the secret.
  name: schema_name
  type: string
provider_name: Snowflake
provider_slug: snowflake
schema_file: json-schema/notification-integration-webhook-secret-schema.json
slug: notification-integration-webhook-secret
source_filename: notification-integration-webhook-secret-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"WebhookSecret\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the secret.\"\n    },\n    \"database_name\": {\n      \"type\": \"string\",\n      \"description\": \"The database which stores the secret.\"\n    },\n    \"schema_name\": {\n      \"type\": \"string\",\n      \"description\": \"The schema which stores the secret.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/snowflake/refs/heads/main/json-schema/notification-integration-webhook-secret-schema.json
tags:
- Data Lakes
- Data Sharing
- Data Warehousing
- Database
- SQL
title: WebhookSecret
---
