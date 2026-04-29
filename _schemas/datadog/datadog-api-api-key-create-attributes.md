---
description: Attributes used to create an API Key.
layout: schema
name: APIKeyCreateAttributes
properties_list:
- description: The APIKeyCreateAttributes category.
  name: category
  type: string
- description: Name of the API key.
  name: name
  type: string
- description: The APIKeyCreateAttributes remote_config_read_enabled.
  name: remote_config_read_enabled
  type: boolean
provider_name: Datadog
provider_slug: datadog
schema_file: json-schema/datadog-api-api-key-create-attributes-schema.json
slug: datadog-api-api-key-create-attributes
source_filename: datadog-api-api-key-create-attributes-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/datadog/refs/heads/main/json-schema/datadog-api-api-key-create-attributes-schema.json\",\n  \"title\": \"APIKeyCreateAttributes\",\n  \"description\": \"Attributes used to create an API Key.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"category\": {\n      \"description\": \"The APIKeyCreateAttributes category.\",\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"name\": {\n      \"description\": \"Name of the API key.\",\n      \"example\": \"API Key for submitting metrics\",\n      \"type\": \"string\"\n    },\n    \"remote_config_read_enabled\": {\n      \"description\": \"The APIKeyCreateAttributes remote_config_read_enabled.\",\n      \"type\": \"boolean\",\n      \"example\": true\n    }\n  },\n  \"required\": [\n    \"name\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/datadog/refs/heads/main/json-schema/datadog-api-api-key-create-attributes-schema.json
tags:
- Analytics
- Dashboards
- Monitoring
- Platform
- T1
- Visualizations
title: APIKeyCreateAttributes
---
