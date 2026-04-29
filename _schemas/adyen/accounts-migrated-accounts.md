---
description: MigratedAccounts schema from Adyen API
layout: schema
name: MigratedAccounts
properties_list:
- description: The unique identifier of the account of the migrated account holder in the balance platform.
  name: balanceAccountId
  type: string
- description: The unique identifier of the account of the migrated account holder in the classic integration.
  name: virtualAccountCode
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/accounts-migrated-accounts-schema.json
slug: accounts-migrated-accounts
source_filename: accounts-migrated-accounts-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/accounts-migrated-accounts-schema.json\",\n  \"title\": \"MigratedAccounts\",\n  \"description\": \"MigratedAccounts schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"balanceAccountId\": {\n      \"description\": \"The unique identifier of the account of the migrated account holder in the balance platform.\",\n      \"type\": \"string\"\n    },\n    \"virtualAccountCode\": {\n      \"description\": \"The unique identifier of the account of the migrated account holder in the classic integration.\",\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/accounts-migrated-accounts-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: MigratedAccounts
---
