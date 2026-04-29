---
description: List of API keys for the developer account.
layout: schema
name: ApiKeysResponse
properties_list:
- description: Array of API keys.
  name: keys
  type: array
provider_name: Biogen
provider_slug: biogen
schema_file: json-schema/biogen-api-keys-response-schema.json
slug: biogen-api-keys-response
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"ApiKeysResponse\",\n  \"type\": \"object\",\n  \"description\": \"List of API keys for the developer account.\",\n  \"properties\": {\n    \"keys\": {\n      \"type\": \"array\",\n      \"description\": \"Array of API keys.\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/ApiKey\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/biogen/refs/heads/main/json-schema/biogen-api-keys-response-schema.json
tags:
- Biotechnology
- Healthcare
- Life Sciences
- Pharmaceuticals
- Neurology
title: ApiKeysResponse
---
