---
description: For each stored value card loaded or reloaded, in the StoredValue response message. Result of loading/reloading a stored value card..
layout: schema
name: StoredValueResult
properties_list:
- description: ''
  name: StoredValueTransactionType
  type: object
- description: Copy.
  name: ProductCode
  type: integer
- description: Copy.
  name: EanUpc
  type: integer
- description: Total amount of the item line.
  name: ItemAmount
  type: number
- description: Copy.
  name: Currency
  type: string
- description: ''
  name: StoredValueAccountStatus
  type: object
- description: ''
  name: HostTransactionID
  type: object
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/terminal-stored-value-result-schema.json
slug: terminal-stored-value-result
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/terminal-stored-value-result-schema.json\",\n  \"title\": \"StoredValueResult\",\n  \"description\": \"For each stored value card loaded or reloaded, in the StoredValue response message. Result of loading/reloading a stored value card..\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"StoredValueTransactionType\": {\n      \"$ref\": \"#/components/schemas/StoredValueTransactionType\"\n    },\n    \"ProductCode\": {\n      \"type\": \"integer\",\n      \"minimum\": 1,\n      \"maximum\": 20,\n      \"description\": \"Copy.\"\n    },\n    \"EanUpc\": {\n      \"type\": \"integer\",\n      \"description\": \"Copy.\"\n    },\n    \"ItemAmount\": {\n      \"type\": \"number\",\n      \"maximum\": 99999999.999999,\n      \"minimum\": 0,\n      \"description\": \"Total amount of the item line.\"\n    },\n    \"\
  Currency\": {\n      \"type\": \"string\",\n      \"pattern\": \"^[A-Z]{3,3}$\",\n      \"description\": \"Copy.\"\n    },\n    \"StoredValueAccountStatus\": {\n      \"$ref\": \"#/components/schemas/StoredValueAccountStatus\"\n    },\n    \"HostTransactionID\": {\n      \"$ref\": \"#/components/schemas/TransactionIDType\"\n    }\n  },\n  \"required\": [\n    \"StoredValueTransactionType\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/terminal-stored-value-result-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: StoredValueResult
---
