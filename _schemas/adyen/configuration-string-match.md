---
description: StringMatch schema from Adyen API
layout: schema
name: StringMatch
properties_list:
- description: 'The type of string matching operation. Possible values: **startsWith**, **endsWith**, **isEqualTo**, **contains**,'
  name: operation
  type: string
- description: The string to be matched.
  name: value
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/configuration-string-match-schema.json
slug: configuration-string-match
source_filename: configuration-string-match-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/configuration-string-match-schema.json\",\n  \"title\": \"StringMatch\",\n  \"description\": \"StringMatch schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"operation\": {\n      \"description\": \"The type of string matching operation. Possible values:  **startsWith**, **endsWith**, **isEqualTo**, **contains**,\",\n      \"enum\": [\n        \"contains\",\n        \"endsWith\",\n        \"isEqualTo\",\n        \"startsWith\"\n      ],\n      \"type\": \"string\"\n    },\n    \"value\": {\n      \"description\": \"The string to be matched.\",\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/configuration-string-match-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: StringMatch
---
