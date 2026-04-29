---
description: List of crop types supported by the Agrio diagnosis service.
layout: schema
name: Supported Crops Response
properties_list:
- description: ''
  name: crops
  type: array
provider_name: agrio
provider_slug: agrio
schema_file: json-schema/agrio-supported-crops-response-schema.json
slug: agrio-supported-crops-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/agrio/refs/heads/main/json-schema/agrio-supported-crops-response-schema.json\",\n  \"title\": \"Supported Crops Response\",\n  \"description\": \"List of crop types supported by the Agrio diagnosis service.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"crops\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/Crop\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/agrio/refs/heads/main/json-schema/agrio-supported-crops-response-schema.json
tags:
- Agriculture
- Plant Disease
- Pest Detection
- AI
- Crop Advisory
title: Supported Crops Response
---
