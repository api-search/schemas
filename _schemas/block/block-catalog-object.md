---
description: The wrapper object for catalog entries of a given object type.
layout: schema
name: CatalogObject
properties_list:
- description: The type of this object.
  name: type
  type: string
- description: Unique ID for this CatalogObject.
  name: id
  type: string
- description: The version of the object for optimistic concurrency control.
  name: version
  type: integer
- description: Structured data for a CatalogItem.
  name: item_data
  type: object
provider_name: Block
provider_slug: block
schema_file: json-schema/block-catalog-object-schema.json
slug: block-catalog-object
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/block/main/json-schema/block-catalog-object-schema.json\",\n  \"title\": \"CatalogObject\",\n  \"description\": \"The wrapper object for catalog entries of a given object type.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"The type of this object.\",\n      \"enum\": [\"ITEM\", \"ITEM_VARIATION\", \"CATEGORY\", \"TAX\", \"DISCOUNT\", \"MODIFIER_LIST\", \"MODIFIER\"],\n      \"example\": \"ITEM\"\n    },\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique ID for this CatalogObject.\",\n      \"example\": \"RYOIMONN5KRSWHVY7TNKH\"\n    },\n    \"version\": {\n      \"type\": \"integer\",\n      \"description\": \"The version of the object for optimistic concurrency control.\",\n      \"example\": 1554399346626\n    },\n    \"item_data\": {\n      \"\
  type\": \"object\",\n      \"description\": \"Structured data for a CatalogItem.\",\n      \"properties\": {\n        \"name\": { \"type\": \"string\", \"example\": \"Caramel Macchiato\" },\n        \"description\": { \"type\": \"string\", \"example\": \"Hot or iced espresso beverage\" }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/block/refs/heads/main/json-schema/block-catalog-object-schema.json
tags:
- Commerce
- Cryptocurrency
- eCommerce
- Fintech
- Payments
- Point Of Sale
- Square
title: CatalogObject
---
