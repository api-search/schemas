---
description: A list of configured stream options for a connection.
layout: schema
name: StreamConfigurations
properties_list:
- description: ''
  name: streams
  type: array
provider_name: Airbyte
provider_slug: airbyte
schema_file: json-schema/airbyte-stream-configurations-schema.json
slug: airbyte-stream-configurations
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/airbyte/refs/heads/main/json-schema/airbyte-stream-configurations-schema.json\",\n  \"title\": \"StreamConfigurations\",\n  \"description\": \"A list of configured stream options for a connection.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"streams\": {\n      \"type\": \"array\",\n      \"format\": \"set\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/StreamConfiguration\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/airbyte/refs/heads/main/json-schema/airbyte-stream-configurations-schema.json
tags:
- Data Integration
- ETL
- ELT
- Open Source
- Data Pipeline
- Connectors
- Data
title: StreamConfigurations
---
