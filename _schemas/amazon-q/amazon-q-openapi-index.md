---
description: Index schema from openapi
layout: schema
name: Index
properties_list:
- description: The unique identifier of the index.
  name: indexId
  type: string
- description: The name of the index.
  name: displayName
  type: string
- description: The status of the index.
  name: status
  type: string
provider_name: Amazon Q
provider_slug: amazon-q
schema_file: json-schema/amazon-q-openapi-index-schema.json
slug: amazon-q-openapi-index
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-q/refs/heads/main/json-schema/amazon-q-openapi-index-schema.json\",\n  \"title\": \"Index\",\n  \"description\": \"Index schema from openapi\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"indexId\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier of the index.\"\n    },\n    \"displayName\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the index.\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"CREATING\",\n        \"ACTIVE\",\n        \"DELETING\",\n        \"FAILED\",\n        \"UPDATING\"\n      ],\n      \"description\": \"The status of the index.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-q/refs/heads/main/json-schema/amazon-q-openapi-index-schema.json
tags:
- Artificial Intelligence
- Assistant
- AWS
- Enterprise
- Generative AI
title: Index
---
