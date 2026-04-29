---
description: 'It contains: - the identification of the stored value accounts or the stored value cards, if provided by the Sale System, and - the associated products sold by the Sale System.. Data related to the stored value card.'
layout: schema
name: StoredValueData
properties_list:
- description: If more than one provider to manage on the POI, and StoredValueAccountID absent.
  name: StoredValueProvider
  type: string
- description: ''
  name: StoredValueTransactionType
  type: object
- description: ''
  name: StoredValueAccountID
  type: object
- description: ''
  name: OriginalPOITransaction
  type: object
- description: Product code of item purchased with the transaction.
  name: ProductCode
  type: integer
- description: Standard product code of item purchased with the transaction.
  name: EanUpc
  type: integer
- description: Total amount of the item line.
  name: ItemAmount
  type: number
- description: Currency of a monetary amount.
  name: Currency
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/terminal-stored-value-data-schema.json
slug: terminal-stored-value-data
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/terminal-stored-value-data-schema.json\",\n  \"title\": \"StoredValueData\",\n  \"description\": \"It contains: - the identification of the stored value accounts or the stored value cards, if provided by the Sale System, and - the associated products sold by the Sale System.. Data related to the stored value card.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"StoredValueProvider\": {\n      \"type\": \"string\",\n      \"pattern\": \"^.+$\",\n      \"description\": \"If more than one provider to manage on the POI, and StoredValueAccountID absent.\"\n    },\n    \"StoredValueTransactionType\": {\n      \"$ref\": \"#/components/schemas/StoredValueTransactionType\"\n    },\n    \"StoredValueAccountID\": {\n      \"$ref\": \"#/components/schemas/StoredValueAccountID\"\n    },\n    \"OriginalPOITransaction\"\
  : {\n      \"$ref\": \"#/components/schemas/OriginalPOITransaction\"\n    },\n    \"ProductCode\": {\n      \"type\": \"integer\",\n      \"minimum\": 1,\n      \"maximum\": 20,\n      \"description\": \"Product code of item purchased with the transaction.\"\n    },\n    \"EanUpc\": {\n      \"type\": \"integer\",\n      \"description\": \"Standard product code of item purchased with the transaction.\"\n    },\n    \"ItemAmount\": {\n      \"type\": \"number\",\n      \"maximum\": 99999999.999999,\n      \"minimum\": 0,\n      \"description\": \"Total amount of the item line.\"\n    },\n    \"Currency\": {\n      \"type\": \"string\",\n      \"pattern\": \"^[A-Z]{3,3}$\",\n      \"description\": \"Currency of a monetary amount.\"\n    }\n  },\n  \"required\": [\n    \"StoredValueTransactionType\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/terminal-stored-value-data-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: StoredValueData
---
