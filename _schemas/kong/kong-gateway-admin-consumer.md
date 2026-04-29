---
description: A Consumer represents a developer or machine using the API. Consumers are used with authentication plugins to identify and control API access.
layout: schema
name: Consumer
properties_list:
- description: The unique identifier of the Consumer.
  name: id
  type: string
- description: The unique username of the Consumer. At least one of username or custom_id must be specified.
  name: username
  type: string
- description: A custom identifier for the Consumer. At least one of username or custom_id must be specified.
  name: custom_id
  type: string
- description: An optional set of strings for grouping and filtering.
  name: tags
  type: array
- description: Unix epoch timestamp of when the entity was created.
  name: created_at
  type: integer
- description: Unix epoch timestamp of when the entity was last updated.
  name: updated_at
  type: integer
provider_name: Kong
provider_slug: kong
schema_file: json-schema/kong-gateway-admin-consumer-schema.json
slug: kong-gateway-admin-consumer
source_filename: kong-gateway-admin-consumer-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Consumer\",\n  \"type\": \"object\",\n  \"description\": \"A Consumer represents a developer or machine using the API. Consumers are used with authentication plugins to identify and control API access.\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier of the Consumer.\"\n    },\n    \"username\": {\n      \"type\": \"string\",\n      \"description\": \"The unique username of the Consumer. At least one of username or custom_id must be specified.\"\n    },\n    \"custom_id\": {\n      \"type\": \"string\",\n      \"description\": \"A custom identifier for the Consumer. At least one of username or custom_id must be specified.\"\n    },\n    \"tags\": {\n      \"type\": \"array\",\n      \"description\": \"An optional set of strings for grouping and filtering.\"\n    },\n    \"created_at\": {\n      \"type\": \"integer\",\n      \"\
  description\": \"Unix epoch timestamp of when the entity was created.\"\n    },\n    \"updated_at\": {\n      \"type\": \"integer\",\n      \"description\": \"Unix epoch timestamp of when the entity was last updated.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/kong/refs/heads/main/json-schema/kong-gateway-admin-consumer-schema.json
tags:
- API Gateway
- Lua
- NGINX
- Open Source
title: Consumer
---
