---
description: Referenced schema from Adyen API
layout: schema
name: Referenced
properties_list:
- description: Indicates whether referenced refunds are enabled on the standalone terminal.
  name: enableStandaloneRefunds
  type: boolean
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/management-referenced-schema.json
slug: management-referenced
source_filename: management-referenced-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/management-referenced-schema.json\",\n  \"title\": \"Referenced\",\n  \"description\": \"Referenced schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"enableStandaloneRefunds\": {\n      \"description\": \"Indicates whether referenced refunds are enabled on the standalone terminal.\",\n      \"type\": \"boolean\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/management-referenced-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: Referenced
---
