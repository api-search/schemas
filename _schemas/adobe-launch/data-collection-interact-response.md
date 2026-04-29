---
description: ''
layout: schema
name: InteractResponse
properties_list:
- description: The unique identifier for this request.
  name: requestId
  type: string
- description: Array of service response handles.
  name: handle
  type: array
provider_name: Adobe Launch
provider_slug: adobe-launch
schema_file: json-schema/data-collection-interact-response-schema.json
slug: data-collection-interact-response
source_filename: data-collection-interact-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"InteractResponse\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"requestId\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier for this request.\"\n    },\n    \"handle\": {\n      \"type\": \"array\",\n      \"description\": \"Array of service response handles.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adobe-launch/refs/heads/main/json-schema/data-collection-interact-response-schema.json
tags:
- Data Collection
- Edge Network
- Event Forwarding
- Marketing Technology
- Tag Management
title: InteractResponse
---
