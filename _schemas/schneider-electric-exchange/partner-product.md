---
description: A Schneider Electric product record from the Partner Product Catalog API, including technical specifications, pricing, and availability data.
layout: schema
name: Schneider Electric Partner Product
properties_list:
- description: Schneider Electric commercial reference number (SKU) for the product.
  name: commercialReference
  type: string
- description: Display name of the product.
  name: productName
  type: string
- description: Technical description of the product.
  name: description
  type: string
- description: Product category classification.
  name: category
  type: string
- description: Product range or family name.
  name: range
  type: string
- description: ETIM 10.0 technical classification data.
  name: etim
  type: object
- description: Public list price.
  name: listPrice
  type: object
- description: Partner-specific net price after discounts.
  name: netPrice
  type: object
- description: Stock availability information.
  name: availability
  type: object
- description: Product digital assets.
  name: digitalAssets
  type: object
provider_name: Schneider Electric Exchange
provider_slug: schneider-electric-exchange
schema_file: json-schema/partner-product-schema.json
slug: partner-product
source_filename: partner-product-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-explorer.se.com/schemas/product\",\n  \"title\": \"Schneider Electric Partner Product\",\n  \"description\": \"A Schneider Electric product record from the Partner Product Catalog API, including technical specifications, pricing, and availability data.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"commercialReference\": {\n      \"type\": \"string\",\n      \"description\": \"Schneider Electric commercial reference number (SKU) for the product.\"\n    },\n    \"productName\": {\n      \"type\": \"string\",\n      \"description\": \"Display name of the product.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Technical description of the product.\"\n    },\n    \"category\": {\n      \"type\": \"string\",\n      \"description\": \"Product category classification.\"\n    },\n    \"range\": {\n      \"type\": \"string\",\n      \"description\"\
  : \"Product range or family name.\"\n    },\n    \"etim\": {\n      \"type\": \"object\",\n      \"description\": \"ETIM 10.0 technical classification data.\",\n      \"properties\": {\n        \"classId\": { \"type\": \"string\" },\n        \"className\": { \"type\": \"string\" },\n        \"features\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"featureId\": { \"type\": \"string\" },\n              \"featureName\": { \"type\": \"string\" },\n              \"value\": {},\n              \"unit\": { \"type\": \"string\" }\n            }\n          }\n        }\n      }\n    },\n    \"listPrice\": {\n      \"$ref\": \"#/$defs/Price\",\n      \"description\": \"Public list price.\"\n    },\n    \"netPrice\": {\n      \"$ref\": \"#/$defs/Price\",\n      \"description\": \"Partner-specific net price after discounts.\"\n    },\n    \"availability\": {\n      \"type\": \"object\",\n      \"description\"\
  : \"Stock availability information.\",\n      \"properties\": {\n        \"stockLevel\": { \"type\": \"integer\" },\n        \"availableDate\": { \"type\": \"string\", \"format\": \"date\" },\n        \"warehouse\": { \"type\": \"string\" }\n      }\n    },\n    \"digitalAssets\": {\n      \"type\": \"object\",\n      \"description\": \"Product digital assets.\",\n      \"properties\": {\n        \"images\": {\n          \"type\": \"array\",\n          \"items\": { \"type\": \"string\", \"format\": \"uri\" }\n        },\n        \"datasheet\": { \"type\": \"string\", \"format\": \"uri\" },\n        \"model3d\": { \"type\": \"string\", \"format\": \"uri\" }\n      }\n    }\n  },\n  \"required\": [\"commercialReference\", \"productName\"],\n  \"$defs\": {\n    \"Price\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"amount\": { \"type\": \"number\" },\n        \"currency\": { \"type\": \"string\" },\n        \"unit\": { \"type\": \"string\" }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/schneider-electric-exchange/refs/heads/main/json-schema/partner-product-schema.json
tags:
- Building Automation
- Commerce APIs
- EcoStruxure
- Energy Management
- Industrial IoT
- Schneider Electric
title: Schneider Electric Partner Product
---
