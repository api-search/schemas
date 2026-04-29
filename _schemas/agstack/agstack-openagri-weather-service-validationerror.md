---
description: ''
layout: schema
name: ValidationError
properties_list:
- description: ''
  name: loc
  type: array
- description: ''
  name: msg
  type: string
- description: ''
  name: type
  type: string
provider_name: AgStack Foundation
provider_slug: agstack
schema_file: json-schema/agstack-openagri-weather-service-validationerror-schema.json
slug: agstack-openagri-weather-service-validationerror
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://agstack.org/schemas/ValidationError.json\",\n  \"title\": \"ValidationError\",\n  \"properties\": {\n    \"loc\": {\n      \"items\": {\n        \"anyOf\": [\n          {\n            \"type\": \"string\"\n          },\n          {\n            \"type\": \"integer\"\n          }\n        ]\n      },\n      \"type\": \"array\",\n      \"title\": \"Location\"\n    },\n    \"msg\": {\n      \"type\": \"string\",\n      \"title\": \"Message\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"title\": \"Error Type\"\n    }\n  },\n  \"type\": \"object\",\n  \"required\": [\n    \"loc\",\n    \"msg\",\n    \"type\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/agstack/refs/heads/main/json-schema/agstack-openagri-weather-service-validationerror-schema.json
tags:
- Agriculture
- Linux Foundation
- Open Source
- Geospatial
- Precision Agriculture
- Linked Data
title: ValidationError
---
