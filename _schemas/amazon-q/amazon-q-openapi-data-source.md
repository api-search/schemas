---
description: DataSource schema from openapi
layout: schema
name: DataSource
properties_list:
- description: The unique identifier of the data source.
  name: dataSourceId
  type: string
- description: The name of the data source.
  name: displayName
  type: string
- description: The type of data source connector.
  name: type
  type: string
- description: The status of the data source.
  name: status
  type: string
provider_name: Amazon Q
provider_slug: amazon-q
schema_file: json-schema/amazon-q-openapi-data-source-schema.json
slug: amazon-q-openapi-data-source
source_filename: amazon-q-openapi-data-source-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-q/refs/heads/main/json-schema/amazon-q-openapi-data-source-schema.json\",\n  \"title\": \"DataSource\",\n  \"description\": \"DataSource schema from openapi\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"dataSourceId\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier of the data source.\"\n    },\n    \"displayName\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the data source.\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"The type of data source connector.\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"PENDING_CREATION\",\n        \"CREATING\",\n        \"ACTIVE\",\n        \"DELETING\",\n        \"UPDATING\",\n        \"NEEDS_ATTENTION\",\n        \"FAILED\"\n      ],\n      \"description\": \"The\
  \ status of the data source.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-q/refs/heads/main/json-schema/amazon-q-openapi-data-source-schema.json
tags:
- Artificial Intelligence
- Assistant
- Enterprise
- Generative AI
title: DataSource
---
