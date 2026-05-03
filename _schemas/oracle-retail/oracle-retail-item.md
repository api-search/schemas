---
description: Schema for an Oracle Retail Merchandising Foundation item record representing a sellable product.
layout: schema
name: Oracle Retail Item
properties_list:
- description: Item number (primary key)
  name: item
  type: string
- description: Primary item description
  name: itemDesc
  type: string
- description: Secondary item description
  name: itemDescSecond
  type: string
- description: A=Active, C=Discontinued, D=Deleted
  name: status
  type: string
- description: Department number
  name: dept
  type: integer
- description: Class number within department
  name: class
  type: integer
- description: Subclass number within class
  name: subclass
  type: integer
- description: 'Item type: REG=Regular, CON=Consignment, TFM=Transform, RB=Reference by barcode, SB=Simple pack, T=Template'
  name: itemType
  type: string
- description: Can this item be sold?
  name: sellable
  type: string
- description: Can this item be ordered from suppliers?
  name: orderable
  type: string
- description: Is inventory tracked for this item?
  name: inventoryInd
  type: string
- description: Current unit retail price
  name: unitRetail
  type: number
- description: ISO 4217 currency code
  name: currencyCode
  type: string
- description: Primary supplier number
  name: supplier
  type: integer
- description: ISO country code for country of origin
  name: originCountry
  type: string
- description: Standard unit cost
  name: unitCost
  type: number
- description: B=Buyer pack, V=Vendor pack
  name: packType
  type: string
- description: Date item was created
  name: createDatetime
  type: string
- description: Date item was last updated
  name: lastUpdateDatetime
  type: string
provider_name: Oracle Retail
provider_slug: oracle-retail
schema_file: json-schema/oracle-retail-item-schema.json
slug: oracle-retail-item
source_filename: oracle-retail-item-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/oracle-retail/json-schema/oracle-retail-item-schema.json\",\n  \"title\": \"Oracle Retail Item\",\n  \"description\": \"Schema for an Oracle Retail Merchandising Foundation item record representing a sellable product.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"item\": {\n      \"type\": \"string\",\n      \"maxLength\": 25,\n      \"description\": \"Item number (primary key)\"\n    },\n    \"itemDesc\": {\n      \"type\": \"string\",\n      \"maxLength\": 250,\n      \"description\": \"Primary item description\"\n    },\n    \"itemDescSecond\": {\n      \"type\": \"string\",\n      \"maxLength\": 250,\n      \"description\": \"Secondary item description\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"enum\": [\"A\", \"C\", \"D\"],\n      \"description\": \"A=Active, C=Discontinued, D=Deleted\"\n    },\n    \"dept\": {\n      \"type\"\
  : \"integer\",\n      \"description\": \"Department number\"\n    },\n    \"class\": {\n      \"type\": \"integer\",\n      \"description\": \"Class number within department\"\n    },\n    \"subclass\": {\n      \"type\": \"integer\",\n      \"description\": \"Subclass number within class\"\n    },\n    \"itemType\": {\n      \"type\": \"string\",\n      \"enum\": [\"REG\", \"CON\", \"TFM\", \"RB\", \"SB\", \"T\"],\n      \"description\": \"Item type: REG=Regular, CON=Consignment, TFM=Transform, RB=Reference by barcode, SB=Simple pack, T=Template\"\n    },\n    \"sellable\": {\n      \"type\": \"string\",\n      \"enum\": [\"Y\", \"N\"],\n      \"description\": \"Can this item be sold?\"\n    },\n    \"orderable\": {\n      \"type\": \"string\",\n      \"enum\": [\"Y\", \"N\"],\n      \"description\": \"Can this item be ordered from suppliers?\"\n    },\n    \"inventoryInd\": {\n      \"type\": \"string\",\n      \"enum\": [\"Y\", \"N\"],\n      \"description\": \"Is inventory tracked\
  \ for this item?\"\n    },\n    \"unitRetail\": {\n      \"type\": \"number\",\n      \"description\": \"Current unit retail price\"\n    },\n    \"currencyCode\": {\n      \"type\": \"string\",\n      \"minLength\": 3,\n      \"maxLength\": 3,\n      \"description\": \"ISO 4217 currency code\"\n    },\n    \"supplier\": {\n      \"type\": \"integer\",\n      \"description\": \"Primary supplier number\"\n    },\n    \"originCountry\": {\n      \"type\": \"string\",\n      \"maxLength\": 3,\n      \"description\": \"ISO country code for country of origin\"\n    },\n    \"unitCost\": {\n      \"type\": \"number\",\n      \"description\": \"Standard unit cost\"\n    },\n    \"packType\": {\n      \"type\": \"string\",\n      \"enum\": [\"B\", \"V\"],\n      \"description\": \"B=Buyer pack, V=Vendor pack\"\n    },\n    \"createDatetime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Date item was created\"\n    },\n    \"lastUpdateDatetime\": {\n\
  \      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Date item was last updated\"\n    }\n  },\n  \"required\": [\"item\", \"itemDesc\", \"dept\", \"class\", \"subclass\", \"status\"],\n  \"examples\": [\n    {\n      \"item\": \"100012345\",\n      \"itemDesc\": \"Men's Cotton T-Shirt Blue Large\",\n      \"status\": \"A\",\n      \"dept\": 100,\n      \"class\": 10,\n      \"subclass\": 5,\n      \"itemType\": \"REG\",\n      \"sellable\": \"Y\",\n      \"orderable\": \"Y\",\n      \"inventoryInd\": \"Y\",\n      \"unitRetail\": 24.99,\n      \"currencyCode\": \"USD\",\n      \"supplier\": 5001,\n      \"originCountry\": \"BGD\"\n    }\n  ]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/oracle-retail/refs/heads/main/json-schema/oracle-retail-item-schema.json
tags:
- Retail
- Merchandising
- Order Management
- Pricing
- Inventory
- Point of Sale
- Omnichannel
- Oracle
title: Oracle Retail Item
---
