---
description: Request body for creating a new API key.
layout: schema
name: CreateApiKeyRequest
properties_list:
- description: Display name for the key.
  name: name
  type: string
- description: Optional key description.
  name: description
  type: string
provider_name: Biogen
provider_slug: biogen
schema_file: json-schema/biogen-create-api-key-request-schema.json
slug: biogen-create-api-key-request
source_filename: biogen-create-api-key-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"CreateApiKeyRequest\",\n  \"type\": \"object\",\n  \"description\": \"Request body for creating a new API key.\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Display name for the key.\",\n      \"example\": \"Production Key\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Optional key description.\",\n      \"example\": \"Key for production CCS-CRX integration\"\n    }\n  },\n  \"required\": [\n    \"name\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/biogen/refs/heads/main/json-schema/biogen-create-api-key-request-schema.json
tags:
- Biotechnology
- Healthcare
- Life Sciences
- Pharmaceuticals
- Neurology
title: CreateApiKeyRequest
---
