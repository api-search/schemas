---
description: ''
layout: schema
name: LocationResourceReference
properties_list:
- description: Identifier of the Location.
  name: value
  type: string
- description: The URI corresponding to a SCIM resource that is this Location.
  name: $ref
  type: string
- description: A human-readable name, primarily used for display purposes.
  name: display
  type: string
provider_name: Factset
provider_slug: factset
schema_file: json-schema/factset-procure-to-pay-scim-location-resource-reference-schema.json
slug: factset-procure-to-pay-scim-location-resource-reference
source_filename: factset-procure-to-pay-scim-location-resource-reference-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"LocationResourceReference\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"value\": {\n      \"type\": \"string\",\n      \"description\": \"Identifier of the Location.\"\n    },\n    \"$ref\": {\n      \"type\": \"string\",\n      \"description\": \"The URI corresponding to a SCIM resource that is this Location.\"\n    },\n    \"display\": {\n      \"type\": \"string\",\n      \"description\": \"A human-readable name, primarily used for display purposes.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/factset/refs/heads/main/json-schema/factset-procure-to-pay-scim-location-resource-reference-schema.json
tags:
- Financial
- Financial Data
- Investment Analytics
- Market Data
- Portfolio Analytics
- Research
title: LocationResourceReference
---
