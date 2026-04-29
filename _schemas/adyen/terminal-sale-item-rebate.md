---
description: To be differentiated from the award which is the amount or quantity earned on the loyalty account. The awarded amount that is attached to an item as a rebate.
layout: schema
name: SaleItemRebate
properties_list:
- description: Item identification inside a transaction (0 to n).
  name: ItemID
  type: integer
- description: Product code of item purchased with the transaction.
  name: ProductCode
  type: integer
- description: ''
  name: EanUpc
  type: integer
- description: ''
  name: UnitOfMeasure
  type: object
- description: if rebate is additional units.
  name: Quantity
  type: string
- description: if rebate on the line item amount.
  name: ItemAmount
  type: number
- description: If provided by the Acquirer.
  name: RebateLabel
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/terminal-sale-item-rebate-schema.json
slug: terminal-sale-item-rebate
source_filename: terminal-sale-item-rebate-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/terminal-sale-item-rebate-schema.json\",\n  \"title\": \"SaleItemRebate\",\n  \"description\": \"To be differentiated from the award which is the amount or quantity earned on the loyalty account. The awarded amount that is attached to an item as a rebate.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ItemID\": {\n      \"type\": \"integer\",\n      \"description\": \"Item identification inside a transaction (0 to n).\"\n    },\n    \"ProductCode\": {\n      \"type\": \"integer\",\n      \"minimum\": 1,\n      \"maximum\": 20,\n      \"description\": \"Product code of item purchased with the transaction.\"\n    },\n    \"EanUpc\": {\n      \"type\": \"integer\"\n    },\n    \"UnitOfMeasure\": {\n      \"$ref\": \"#/components/schemas/UnitOfMeasure\"\n    },\n    \"Quantity\": {\n      \"type\": \"string\"\
  ,\n      \"description\": \"if rebate is additional units.\"\n    },\n    \"ItemAmount\": {\n      \"type\": \"number\",\n      \"maximum\": 99999999.999999,\n      \"minimum\": 0,\n      \"description\": \"if rebate on the line item amount.\"\n    },\n    \"RebateLabel\": {\n      \"type\": \"string\",\n      \"pattern\": \"^.+$\",\n      \"description\": \"If provided by the Acquirer.\"\n    }\n  },\n  \"required\": [\n    \"ItemID\",\n    \"ProductCode\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/terminal-sale-item-rebate-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: SaleItemRebate
---
