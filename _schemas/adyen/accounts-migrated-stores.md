---
description: MigratedStores schema from Adyen API
layout: schema
name: MigratedStores
properties_list:
- description: The unique identifier of the business line associated with the migrated account holder in the balance platform.
  name: businessLineId
  type: string
- description: The unique identifier of the store associated with the migrated account holder in the classic integration.
  name: storeCode
  type: string
- description: The unique identifier of the store associated with the migrated account holder in the balance platform.
  name: storeId
  type: string
- description: Your reference for the store in the classic integration. The [Customer Area](https://ca-test.adyen.com/) uses this value for the store description.
  name: storeReference
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/accounts-migrated-stores-schema.json
slug: accounts-migrated-stores
source_filename: accounts-migrated-stores-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/accounts-migrated-stores-schema.json\",\n  \"title\": \"MigratedStores\",\n  \"description\": \"MigratedStores schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"businessLineId\": {\n      \"description\": \"The unique identifier of the business line associated with the migrated account holder in the balance platform.\",\n      \"type\": \"string\"\n    },\n    \"storeCode\": {\n      \"description\": \"The unique identifier of the store associated with the migrated account holder in the classic integration.\",\n      \"type\": \"string\"\n    },\n    \"storeId\": {\n      \"description\": \"The unique identifier of the store associated with the migrated account holder in the balance platform.\",\n      \"type\": \"string\"\n    },\n    \"storeReference\": {\n      \"description\": \"\
  Your reference for the store in the classic integration. The [Customer Area](https://ca-test.adyen.com/) uses this value for the store description.\",\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/accounts-migrated-stores-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: MigratedStores
---
