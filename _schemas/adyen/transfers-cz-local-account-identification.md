---
description: CZLocalAccountIdentification schema from Adyen API
layout: schema
name: CZLocalAccountIdentification
properties_list:
- description: 'The 2- to 16-digit bank account number (Číslo účtu) in the following format: - The optional prefix (předčíslí). - The required second part (základní část) which must be at least two non-zero digits. E'
  name: accountNumber
  type: string
- description: The 4-digit bank code (Kód banky), without separators or whitespace.
  name: bankCode
  type: string
- description: '**czLocal**'
  name: type
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/transfers-cz-local-account-identification-schema.json
slug: transfers-cz-local-account-identification
source_filename: transfers-cz-local-account-identification-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/transfers-cz-local-account-identification-schema.json\",\n  \"title\": \"CZLocalAccountIdentification\",\n  \"description\": \"CZLocalAccountIdentification schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"accountNumber\": {\n      \"description\": \"The 2- to 16-digit bank account number (\\u010c\\u00edslo \\u00fa\\u010dtu) in the following format:\\n\\n- The optional prefix (p\\u0159ed\\u010d\\u00edsl\\u00ed).\\n\\n- The required second part (z\\u00e1kladn\\u00ed \\u010d\\u00e1st) which must be at least two non-zero digits.\\n\\nExamples:\\n\\n- **19-123457** (with prefix)\\n\\n- **123457** (without prefix)\\n\\n- **000019-0000123457** (with prefix, normalized)\\n\\n- **000000-0000123457** (without prefix, normalized)\",\n      \"maxLength\": 17,\n      \"minLength\": 2,\n      \"type\"\
  : \"string\"\n    },\n    \"bankCode\": {\n      \"description\": \"The 4-digit bank code (K\\u00f3d banky), without separators or whitespace.\",\n      \"maxLength\": 4,\n      \"minLength\": 4,\n      \"type\": \"string\"\n    },\n    \"type\": {\n      \"default\": \"czLocal\",\n      \"description\": \"**czLocal**\",\n      \"enum\": [\n        \"czLocal\"\n      ],\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"type\",\n    \"accountNumber\",\n    \"bankCode\"\n  ],\n  \"additionalProperties\": false\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/transfers-cz-local-account-identification-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: CZLocalAccountIdentification
---
