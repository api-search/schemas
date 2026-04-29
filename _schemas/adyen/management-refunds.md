---
description: Refunds schema from Adyen API
layout: schema
name: Refunds
properties_list:
- description: Settings for referenced refunds.
  name: referenced
  type: object
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/management-refunds-schema.json
slug: management-refunds
source_filename: management-refunds-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/management-refunds-schema.json\",\n  \"title\": \"Refunds\",\n  \"description\": \"Refunds schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"referenced\": {\n      \"description\": \"Settings for referenced refunds.\",\n      \"$ref\": \"#/components/schemas/Referenced\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/management-refunds-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: Refunds
---
