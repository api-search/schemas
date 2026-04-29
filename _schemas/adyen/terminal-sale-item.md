---
description: In loyalty or value added payment card transaction, the items of the sale are entering in the processing of the transaction. Sale items of a transaction.
layout: schema
name: SaleItem
properties_list:
- description: Item identification inside a transaction (0 to n).
  name: ItemID
  type: integer
- description: Product code of item purchased with the transaction.
  name: ProductCode
  type: integer
- description: If data sent, POI has to store it and send it if the host protocol allows it.
  name: EanUpc
  type: integer
- description: ''
  name: UnitOfMeasure
  type: object
- description: If data sent, POI has to store it and send it if the host protocol allows it.
  name: Quantity
  type: string
- description: if Quantity present.
  name: UnitPrice
  type: number
- description: Total amount of the item line.
  name: ItemAmount
  type: number
- description: If data sent, POI has to store it and send it if the host protocol allows it.
  name: TaxCode
  type: integer
- description: If data sent, POI has to store it and send it if the host protocol allows it.
  name: SaleChannel
  type: integer
- description: ''
  name: ProductLabel
  type: string
- description: If data sent, POI has to store it and send it if the host protocol allows it.
  name: AdditionalProductInfo
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/terminal-sale-item-schema.json
slug: terminal-sale-item
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/terminal-sale-item-schema.json\",\n  \"title\": \"SaleItem\",\n  \"description\": \"In loyalty or value added payment card transaction, the items of the sale are entering in the processing of the transaction. Sale items of a transaction.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ItemID\": {\n      \"type\": \"integer\",\n      \"description\": \"Item identification inside a transaction (0 to n).\"\n    },\n    \"ProductCode\": {\n      \"type\": \"integer\",\n      \"minimum\": 1,\n      \"maximum\": 20,\n      \"description\": \"Product code of item purchased with the transaction.\"\n    },\n    \"EanUpc\": {\n      \"type\": \"integer\",\n      \"description\": \"If data sent, POI has to store it and send it if the host protocol allows it.\"\n    },\n    \"UnitOfMeasure\": {\n      \"$ref\": \"#/components/schemas/UnitOfMeasure\"\
  \n    },\n    \"Quantity\": {\n      \"type\": \"string\",\n      \"description\": \"If data sent, POI has to store it and send it if the host protocol allows it.\"\n    },\n    \"UnitPrice\": {\n      \"type\": \"number\",\n      \"maximum\": 99999999.999999,\n      \"minimum\": 0,\n      \"description\": \"if Quantity present.\"\n    },\n    \"ItemAmount\": {\n      \"type\": \"number\",\n      \"maximum\": 99999999.999999,\n      \"minimum\": 0,\n      \"description\": \"Total amount of the item line.\"\n    },\n    \"TaxCode\": {\n      \"type\": \"integer\",\n      \"description\": \"If data sent, POI has to store it and send it if the host protocol allows it.\"\n    },\n    \"SaleChannel\": {\n      \"type\": \"integer\",\n      \"description\": \"If data sent, POI has to store it and send it if the host protocol allows it.\"\n    },\n    \"ProductLabel\": {\n      \"type\": \"string\",\n      \"pattern\": \"^.+$\"\n    },\n    \"AdditionalProductInfo\": {\n      \"type\": \"string\"\
  ,\n      \"pattern\": \"^.+$\",\n      \"description\": \"If data sent, POI has to store it and send it if the host protocol allows it.\"\n    }\n  },\n  \"required\": [\n    \"ItemID\",\n    \"ProductCode\",\n    \"ItemAmount\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/terminal-sale-item-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: SaleItem
---
