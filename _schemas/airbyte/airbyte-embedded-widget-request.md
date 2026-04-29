---
description: EmbeddedWidgetRequest schema from Airbyte API
layout: schema
name: EmbeddedWidgetRequest
properties_list:
- description: ''
  name: allowedOrigin
  type: string
- description: ''
  name: externalUserId
  type: string
- description: ''
  name: organizationId
  type: string
provider_name: Airbyte
provider_slug: airbyte
schema_file: json-schema/airbyte-embedded-widget-request-schema.json
slug: airbyte-embedded-widget-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/airbyte/refs/heads/main/json-schema/airbyte-embedded-widget-request-schema.json\",\n  \"title\": \"EmbeddedWidgetRequest\",\n  \"description\": \"EmbeddedWidgetRequest schema from Airbyte API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"allowedOrigin\": {\n      \"type\": \"string\"\n    },\n    \"externalUserId\": {\n      \"type\": \"string\"\n    },\n    \"organizationId\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\"\n    }\n  },\n  \"required\": [\n    \"allowedOrigin\",\n    \"externalUserId\",\n    \"organizationId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/airbyte/refs/heads/main/json-schema/airbyte-embedded-widget-request-schema.json
tags:
- Data Integration
- ETL
- ELT
- Open Source
- Data Pipeline
- Connectors
- Data
title: EmbeddedWidgetRequest
---
