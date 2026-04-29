---
description: Information about the user who created the monitor
layout: schema
name: Creator
properties_list:
- description: The unique numeric ID of the creator user
  name: id
  type: integer
- description: The display name of the creator user
  name: name
  type: string
- description: The email address of the creator user
  name: email
  type: string
- description: The Datadog handle (username) of the creator user
  name: handle
  type: string
provider_name: Datadog
provider_slug: datadog
schema_file: json-schema/datadog-monitors-creator-schema.json
slug: datadog-monitors-creator
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/datadog/refs/heads/main/json-schema/datadog-monitors-creator-schema.json\",\n  \"title\": \"Creator\",\n  \"description\": \"Information about the user who created the monitor\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"integer\",\n      \"description\": \"The unique numeric ID of the creator user\",\n      \"example\": 42\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The display name of the creator user\",\n      \"example\": \"Example Monitor\"\n    },\n    \"email\": {\n      \"type\": \"string\",\n      \"format\": \"email\",\n      \"description\": \"The email address of the creator user\",\n      \"example\": \"user@example.com\"\n    },\n    \"handle\": {\n      \"type\": \"string\",\n      \"description\": \"The Datadog handle (username) of the creator user\",\n   \
  \   \"example\": \"example_value\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/datadog/refs/heads/main/json-schema/datadog-monitors-creator-schema.json
tags:
- Analytics
- Dashboards
- Monitoring
- Platform
- T1
- Visualizations
title: Creator
---
