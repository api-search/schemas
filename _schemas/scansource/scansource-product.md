---
description: A product in the ScanSource technology distribution catalog including specifications, pricing, and inventory data.
layout: schema
name: ScanSource Product
properties_list:
- description: ScanSource internal item number
  name: itemNumber
  type: string
- description: Manufacturer's part number
  name: manufacturerPartNumber
  type: string
- description: Manufacturer name
  name: manufacturer
  type: string
- description: Product description
  name: description
  type: string
- description: Product category hierarchy path
  name: categoryPath
  type: string
- description: Universal Product Code (UPC)
  name: upc
  type: string
- description: Indicates whether the product has been discontinued
  name: isObsolete
  type: boolean
- description: Product weight in pounds
  name: weight
  type: number
- description: Product physical dimensions
  name: dimensions
  type: object
- description: Technical specifications as key-value pairs
  name: specifications
  type: object
- description: Pricing information for the product
  name: pricing
  type: object
- description: Real-time inventory availability
  name: availability
  type: object
provider_name: ScanSource
provider_slug: scansource
schema_file: json-schema/scansource-product-schema.json
slug: scansource-product
source_filename: scansource-product-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"$id\": \"https://github.com/api-evangelist/scansource/blob/main/json-schema/scansource-product-schema.json\",\n  \"title\": \"ScanSource Product\",\n  \"description\": \"A product in the ScanSource technology distribution catalog including specifications, pricing, and inventory data.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"itemNumber\": {\n      \"type\": \"string\",\n      \"description\": \"ScanSource internal item number\"\n    },\n    \"manufacturerPartNumber\": {\n      \"type\": \"string\",\n      \"description\": \"Manufacturer's part number\"\n    },\n    \"manufacturer\": {\n      \"type\": \"string\",\n      \"description\": \"Manufacturer name\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Product description\"\n    },\n    \"categoryPath\": {\n      \"type\": \"string\",\n      \"description\": \"Product category hierarchy path\"\n    },\n\
  \    \"upc\": {\n      \"type\": \"string\",\n      \"description\": \"Universal Product Code (UPC)\"\n    },\n    \"isObsolete\": {\n      \"type\": \"boolean\",\n      \"description\": \"Indicates whether the product has been discontinued\"\n    },\n    \"weight\": {\n      \"type\": \"number\",\n      \"description\": \"Product weight in pounds\"\n    },\n    \"dimensions\": {\n      \"type\": \"object\",\n      \"description\": \"Product physical dimensions\",\n      \"properties\": {\n        \"length\": { \"type\": \"number\", \"description\": \"Length in inches\" },\n        \"width\": { \"type\": \"number\", \"description\": \"Width in inches\" },\n        \"height\": { \"type\": \"number\", \"description\": \"Height in inches\" }\n      }\n    },\n    \"specifications\": {\n      \"type\": \"object\",\n      \"description\": \"Technical specifications as key-value pairs\",\n      \"additionalProperties\": { \"type\": \"string\" }\n    },\n    \"pricing\": {\n      \"type\": \"\
  object\",\n      \"description\": \"Pricing information for the product\",\n      \"properties\": {\n        \"unitPrice\": { \"type\": \"number\", \"description\": \"Base unit price\" },\n        \"currency\": { \"type\": \"string\", \"default\": \"USD\" },\n        \"priceBreaks\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"quantity\": { \"type\": \"integer\" },\n              \"price\": { \"type\": \"number\" }\n            }\n          }\n        }\n      }\n    },\n    \"availability\": {\n      \"type\": \"object\",\n      \"description\": \"Real-time inventory availability\",\n      \"properties\": {\n        \"quantityAvailable\": { \"type\": \"integer\" },\n        \"warehouse\": { \"type\": \"string\" },\n        \"estimatedShipDate\": { \"type\": \"string\", \"format\": \"date\" }\n      }\n    }\n  },\n  \"required\": [\"itemNumber\", \"manufacturer\", \"description\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/scansource/refs/heads/main/json-schema/scansource-product-schema.json
tags:
- ScanSource
- Distribution
- Barcode
- Point Of Sale
- AIDC
- Inventory
- Order Management
- E-Commerce
title: ScanSource Product
---
