---
description: Schema for a product catalog item in the Rithum Dsco platform.
layout: schema
name: Dsco Catalog Item
properties_list:
- description: Supplier stock keeping unit identifier
  name: sku
  type: string
- description: Product title
  name: title
  type: string
- description: Product description
  name: description
  type: string
- description: Wholesale cost — required for dropship model
  name: cost
  type: number
- description: Rules governing which retail models this item supports
  name: retailModelRules
  type: object
- description: Arbitrary product attributes (color, size, weight, etc.)
  name: attributes
  type: object
provider_name: Rithum
provider_slug: rithum
schema_file: json-schema/dsco-catalog-item-schema.json
slug: dsco-catalog-item
source_filename: dsco-catalog-item-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"$id\": \"https://api-evangelist.github.io/rithum/json-schema/dsco-catalog-item-schema.json\",\n  \"title\": \"Dsco Catalog Item\",\n  \"description\": \"Schema for a product catalog item in the Rithum Dsco platform.\",\n  \"type\": \"object\",\n  \"required\": [\"sku\"],\n  \"properties\": {\n    \"sku\": {\n      \"type\": \"string\",\n      \"description\": \"Supplier stock keeping unit identifier\"\n    },\n    \"title\": {\n      \"type\": \"string\",\n      \"description\": \"Product title\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Product description\"\n    },\n    \"cost\": {\n      \"type\": \"number\",\n      \"format\": \"float\",\n      \"description\": \"Wholesale cost — required for dropship model\"\n    },\n    \"retailModelRules\": {\n      \"type\": \"object\",\n      \"description\": \"Rules governing which retail models this item supports\",\n\
  \      \"properties\": {\n        \"allowedModels\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"string\",\n            \"enum\": [\"dropship\", \"marketplace\"]\n          },\n          \"description\": \"Must include 'dropship' to enable dropship usage\"\n        }\n      }\n    },\n    \"attributes\": {\n      \"type\": \"object\",\n      \"description\": \"Arbitrary product attributes (color, size, weight, etc.)\",\n      \"additionalProperties\": true\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/rithum/refs/heads/main/json-schema/dsco-catalog-item-schema.json
tags:
- Commerce
- Dropship
- Marketplace
- Ecommerce
- Supply Chain
- Retail
title: Dsco Catalog Item
---
