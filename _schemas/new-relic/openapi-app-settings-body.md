---
description: AppSettingsBody schema
layout: schema
name: AppSettingsBody
properties_list:
- description: ''
  name: app_apdex_threshold
  type: number
- description: ''
  name: enable_real_user_monitoring
  type: boolean
- description: ''
  name: end_user_apdex_threshold
  type: number
provider_name: New Relic
provider_slug: new-relic
schema_file: json-schema/openapi-app-settings-body-schema.json
slug: openapi-app-settings-body
source_filename: openapi-app-settings-body-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/new-relic/refs/heads/main/json-schema/openapi-app-settings-body-schema.json\",\n  \"title\": \"AppSettingsBody\",\n  \"description\": \"AppSettingsBody schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"app_apdex_threshold\": {\n      \"type\": \"number\",\n      \"format\": \"float\",\n      \"example\": 42.5\n    },\n    \"enable_real_user_monitoring\": {\n      \"type\": \"boolean\",\n      \"example\": true\n    },\n    \"end_user_apdex_threshold\": {\n      \"type\": \"number\",\n      \"format\": \"float\",\n      \"example\": 42.5\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/new-relic/refs/heads/main/json-schema/openapi-app-settings-body-schema.json
tags:
- Analysis
- Analytics
- APM
- DevOps
- Infrastructure
- Monitoring
- Observability
- Performance
- Platform
title: AppSettingsBody
---
