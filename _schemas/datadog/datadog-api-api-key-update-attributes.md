---
description: Attributes used to update an API Key.
layout: schema
name: APIKeyUpdateAttributes
properties_list:
- description: The APIKeyUpdateAttributes category.
  name: category
  type: string
- description: Name of the API key.
  name: name
  type: string
- description: The APIKeyUpdateAttributes remote_config_read_enabled.
  name: remote_config_read_enabled
  type: boolean
provider_name: Datadog
provider_slug: datadog
schema_file: json-schema/datadog-api-api-key-update-attributes-schema.json
slug: datadog-api-api-key-update-attributes
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/datadog/refs/heads/main/json-schema/datadog-api-api-key-update-attributes-schema.json\",\n  \"title\": \"APIKeyUpdateAttributes\",\n  \"description\": \"Attributes used to update an API Key.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"category\": {\n      \"description\": \"The APIKeyUpdateAttributes category.\",\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"name\": {\n      \"description\": \"Name of the API key.\",\n      \"example\": \"API Key for submitting metrics\",\n      \"type\": \"string\"\n    },\n    \"remote_config_read_enabled\": {\n      \"description\": \"The APIKeyUpdateAttributes remote_config_read_enabled.\",\n      \"type\": \"boolean\",\n      \"example\": true\n    }\n  },\n  \"required\": [\n    \"name\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/datadog/refs/heads/main/json-schema/datadog-api-api-key-update-attributes-schema.json
tags:
- Analytics
- Dashboards
- Monitoring
- Platform
- T1
- Visualizations
title: APIKeyUpdateAttributes
---
