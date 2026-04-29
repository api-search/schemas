---
description: The stream properties associated with a connection.
layout: schema
name: StreamProperties
properties_list:
- description: ''
  name: streamName
  type: string
- description: ''
  name: syncModes
  type: array
- description: ''
  name: streamnamespace
  type: string
- description: ''
  name: defaultCursorField
  type: array
- description: ''
  name: sourceDefinedCursorField
  type: boolean
- description: ''
  name: sourceDefinedPrimaryKey
  type: array
- description: ''
  name: propertyFields
  type: array
provider_name: Airbyte
provider_slug: airbyte
schema_file: json-schema/airbyte-stream-properties-schema.json
slug: airbyte-stream-properties
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/airbyte/refs/heads/main/json-schema/airbyte-stream-properties-schema.json\",\n  \"title\": \"StreamProperties\",\n  \"description\": \"The stream properties associated with a connection.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"streamName\": {\n      \"type\": \"string\"\n    },\n    \"syncModes\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/ConnectionSyncModeEnum\"\n      }\n    },\n    \"streamnamespace\": {\n      \"type\": \"string\"\n    },\n    \"defaultCursorField\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"sourceDefinedCursorField\": {\n      \"type\": \"boolean\"\n    },\n    \"sourceDefinedPrimaryKey\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"array\",\n        \"items\": {\n      \
  \    \"type\": \"string\"\n        }\n      }\n    },\n    \"propertyFields\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"array\",\n        \"items\": {\n          \"type\": \"string\"\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/airbyte/refs/heads/main/json-schema/airbyte-stream-properties-schema.json
tags:
- Data Integration
- ETL
- ELT
- Open Source
- Data Pipeline
- Connectors
- Data
title: StreamProperties
---
