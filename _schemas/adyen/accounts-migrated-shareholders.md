---
description: MigratedShareholders schema from Adyen API
layout: schema
name: MigratedShareholders
properties_list:
- description: The unique identifier of the legal entity of that shareholder in the balance platform.
  name: legalEntityCode
  type: string
- description: The unique identifier of the account of the migrated shareholder in the classic integration.
  name: shareholderCode
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/accounts-migrated-shareholders-schema.json
slug: accounts-migrated-shareholders
source_filename: accounts-migrated-shareholders-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/accounts-migrated-shareholders-schema.json\",\n  \"title\": \"MigratedShareholders\",\n  \"description\": \"MigratedShareholders schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"legalEntityCode\": {\n      \"description\": \"The unique identifier of the legal entity of that shareholder in the balance platform.\",\n      \"type\": \"string\"\n    },\n    \"shareholderCode\": {\n      \"description\": \"The unique identifier of the account of the migrated shareholder in the classic integration.\",\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/accounts-migrated-shareholders-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: MigratedShareholders
---
