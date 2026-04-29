---
description: MigrationData schema from Adyen API
layout: schema
name: MigrationData
properties_list:
- description: The unique identifier of the account holder in the balance platform.
  name: accountHolderId
  type: string
- description: The unique identifier of the balance platfrom to which the account holder was migrated.
  name: balancePlatform
  type: string
- description: Set to **true** if the account holder has been migrated.
  name: migrated
  type: boolean
- description: Contains the mapping of virtual account codes (classic integration) to the balance account codes (balance platform) associated with the migrated account holder.
  name: migratedAccounts
  type: array
- description: Contains the mapping of shareholders associated with the migrated legal entities.
  name: migratedShareholders
  type: array
- description: Contains the mapping of business lines and stores associated with the migrated account holder.
  name: migratedStores
  type: array
- description: The date when account holder was migrated.
  name: migrationDate
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/accounts-migration-data-schema.json
slug: accounts-migration-data
source_filename: accounts-migration-data-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/accounts-migration-data-schema.json\",\n  \"title\": \"MigrationData\",\n  \"description\": \"MigrationData schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"accountHolderId\": {\n      \"description\": \"The unique identifier of the account holder in the balance platform.\",\n      \"type\": \"string\"\n    },\n    \"balancePlatform\": {\n      \"description\": \"The unique identifier of the balance platfrom to which the account holder was migrated.\",\n      \"type\": \"string\"\n    },\n    \"migrated\": {\n      \"description\": \"Set to **true** if the account holder has been migrated.\",\n      \"type\": \"boolean\"\n    },\n    \"migratedAccounts\": {\n      \"description\": \"Contains the mapping of virtual account codes (classic integration) to the balance account codes (balance\
  \ platform) associated with the migrated account holder.\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/MigratedAccounts\"\n      },\n      \"type\": \"array\"\n    },\n    \"migratedShareholders\": {\n      \"description\": \"Contains the mapping of shareholders associated with the migrated legal entities.\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/MigratedShareholders\"\n      },\n      \"type\": \"array\"\n    },\n    \"migratedStores\": {\n      \"description\": \"Contains the mapping of business lines and stores associated with the migrated account holder.\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/MigratedStores\"\n      },\n      \"type\": \"array\"\n    },\n    \"migrationDate\": {\n      \"description\": \"The date when account holder was migrated.\",\n      \"format\": \"date-time\",\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/accounts-migration-data-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: MigrationData
---
