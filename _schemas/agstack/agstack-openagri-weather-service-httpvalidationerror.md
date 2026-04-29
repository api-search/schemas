---
description: ''
layout: schema
name: HTTPValidationError
properties_list:
- description: ''
  name: detail
  type: array
provider_name: AgStack Foundation
provider_slug: agstack
schema_file: json-schema/agstack-openagri-weather-service-httpvalidationerror-schema.json
slug: agstack-openagri-weather-service-httpvalidationerror
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://agstack.org/schemas/HTTPValidationError.json\",\n  \"title\": \"HTTPValidationError\",\n  \"properties\": {\n    \"detail\": {\n      \"items\": {\n        \"$ref\": \"#/components/schemas/ValidationError\"\n      },\n      \"type\": \"array\",\n      \"title\": \"Detail\"\n    }\n  },\n  \"type\": \"object\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/agstack/refs/heads/main/json-schema/agstack-openagri-weather-service-httpvalidationerror-schema.json
tags:
- Agriculture
- Linux Foundation
- Open Source
- Geospatial
- Precision Agriculture
- Linked Data
title: HTTPValidationError
---
