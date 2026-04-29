---
description: CountriesRestriction schema from Adyen API
layout: schema
name: CountriesRestriction
properties_list:
- description: Defines how the condition must be evaluated.
  name: operation
  type: string
- description: List of two-character [ISO 3166-1 alpha-2](https://en.wikipedia.org/wiki/ISO_3166-1_alpha-2) country codes.
  name: value
  type: array
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/configuration-countries-restriction-schema.json
slug: configuration-countries-restriction
source_filename: configuration-countries-restriction-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/configuration-countries-restriction-schema.json\",\n  \"title\": \"CountriesRestriction\",\n  \"description\": \"CountriesRestriction schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"operation\": {\n      \"description\": \"Defines how the condition must be evaluated.\",\n      \"type\": \"string\"\n    },\n    \"value\": {\n      \"description\": \"List of two-character [ISO 3166-1 alpha-2](https://en.wikipedia.org/wiki/ISO_3166-1_alpha-2) country codes.\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"type\": \"array\"\n    }\n  },\n  \"required\": [\n    \"operation\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/configuration-countries-restriction-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: CountriesRestriction
---
