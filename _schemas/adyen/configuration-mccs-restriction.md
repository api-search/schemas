---
description: MccsRestriction schema from Adyen API
layout: schema
name: MccsRestriction
properties_list:
- description: Defines how the condition must be evaluated.
  name: operation
  type: string
- description: List of merchant category codes (MCCs).
  name: value
  type: array
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/configuration-mccs-restriction-schema.json
slug: configuration-mccs-restriction
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/configuration-mccs-restriction-schema.json\",\n  \"title\": \"MccsRestriction\",\n  \"description\": \"MccsRestriction schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"operation\": {\n      \"description\": \"Defines how the condition must be evaluated.\",\n      \"type\": \"string\"\n    },\n    \"value\": {\n      \"description\": \"List of merchant category codes (MCCs).\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"type\": \"array\"\n    }\n  },\n  \"required\": [\n    \"operation\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/configuration-mccs-restriction-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: MccsRestriction
---
