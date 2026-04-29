---
description: BalancePlatform schema from Adyen API
layout: schema
name: BalancePlatform
properties_list:
- description: Your description of the balance platform, maximum 300 characters.
  name: description
  type: string
- description: The unique identifier of the balance platform.
  name: id
  type: string
- description: 'The status of the balance platform. Possible values: **Active**, **Inactive**, **Closed**, **Suspended**.'
  name: status
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/configuration-balance-platform-schema.json
slug: configuration-balance-platform
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/configuration-balance-platform-schema.json\",\n  \"title\": \"BalancePlatform\",\n  \"description\": \"BalancePlatform schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"description\": {\n      \"description\": \"Your description of the balance platform, maximum 300 characters.\",\n      \"maxLength\": 300,\n      \"type\": \"string\"\n    },\n    \"id\": {\n      \"description\": \"The unique identifier of the balance platform.\",\n      \"type\": \"string\"\n    },\n    \"status\": {\n      \"description\": \"The status of the balance platform.\\n\\nPossible values: **Active**, **Inactive**, **Closed**, **Suspended**.\",\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"id\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/configuration-balance-platform-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: BalancePlatform
---
