---
description: Commission schema from Adyen API
layout: schema
name: Commission
properties_list:
- description: A fixed commission fee, in minor units.
  name: fixedAmount
  type: integer
- description: A variable commission fee, in basis points.
  name: variablePercentage
  type: integer
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/management-commission-schema.json
slug: management-commission
source_filename: management-commission-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/management-commission-schema.json\",\n  \"title\": \"Commission\",\n  \"description\": \"Commission schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"fixedAmount\": {\n      \"description\": \"A fixed commission fee, in minor units.\",\n      \"format\": \"int64\",\n      \"type\": \"integer\"\n    },\n    \"variablePercentage\": {\n      \"description\": \"A variable commission fee, in basis points.\",\n      \"format\": \"int64\",\n      \"type\": \"integer\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/management-commission-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: Commission
---
