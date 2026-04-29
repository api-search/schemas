---
description: Point schema from Adyen API
layout: schema
name: Point
properties_list:
- description: ''
  name: X
  type: string
- description: ''
  name: Y
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/terminal-point-schema.json
slug: terminal-point
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/terminal-point-schema.json\",\n  \"title\": \"Point\",\n  \"description\": \"Point schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"X\": {\n      \"type\": \"string\"\n    },\n    \"Y\": {\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"X\",\n    \"Y\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/terminal-point-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: Point
---
