---
description: TerminalModelsResponse schema from Adyen API
layout: schema
name: TerminalModelsResponse
properties_list:
- description: The terminal models that the API credential has access to.
  name: data
  type: array
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/management-terminal-models-response-schema.json
slug: management-terminal-models-response
source_filename: management-terminal-models-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/management-terminal-models-response-schema.json\",\n  \"title\": \"TerminalModelsResponse\",\n  \"description\": \"TerminalModelsResponse schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"data\": {\n      \"description\": \"The terminal models that the API credential has access to.\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/IdName\"\n      },\n      \"type\": \"array\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/management-terminal-models-response-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: TerminalModelsResponse
---
