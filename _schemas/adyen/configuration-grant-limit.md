---
description: GrantLimit schema from Adyen API
layout: schema
name: GrantLimit
properties_list:
- description: The amount available on the grant account.
  name: amount
  type: object
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/configuration-grant-limit-schema.json
slug: configuration-grant-limit
source_filename: configuration-grant-limit-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/configuration-grant-limit-schema.json\",\n  \"title\": \"GrantLimit\",\n  \"description\": \"GrantLimit schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"amount\": {\n      \"description\": \"The amount available on the grant account.\",\n      \"$ref\": \"#/components/schemas/Amount\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/configuration-grant-limit-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: GrantLimit
---
