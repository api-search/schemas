---
description: Schema for a recall record returned by the CPSC SaferProducts.gov recalls API.
layout: schema
name: CPSC Recall
properties_list:
- description: ''
  name: RecallID
  type: integer
- description: ''
  name: RecallNumber
  type: string
- description: ''
  name: RecallDate
  type: string
- description: ''
  name: Description
  type: string
- description: ''
  name: URL
  type: string
- description: ''
  name: Title
  type: string
- description: ''
  name: ConsumerContact
  type: string
- description: ''
  name: LastPublishDate
  type: string
- description: ''
  name: Products
  type: array
- description: ''
  name: Inconjunctions
  type: array
- description: ''
  name: Images
  type: array
- description: ''
  name: Injuries
  type: array
- description: ''
  name: Manufacturers
  type: array
- description: ''
  name: Retailers
  type: array
- description: ''
  name: Importers
  type: array
- description: ''
  name: Distributors
  type: array
- description: ''
  name: ManufacturerCountries
  type: array
- description: ''
  name: ProductUPCs
  type: array
- description: ''
  name: Hazards
  type: array
- description: ''
  name: Remedies
  type: array
- description: ''
  name: RemedyOptions
  type: array
provider_name: Consumer Product Safety Commission
provider_slug: consumer-product-safety-commission
schema_file: json-schema/cpsc-recall-schema.json
slug: cpsc-recall
source_filename: cpsc-recall-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/consumer-product-safety-commission/refs/heads/main/json-schema/cpsc-recall-schema.json\",\n  \"title\": \"CPSC Recall\",\n  \"description\": \"Schema for a recall record returned by the CPSC SaferProducts.gov recalls API.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"RecallID\": { \"type\": \"integer\" },\n    \"RecallNumber\": { \"type\": \"string\" },\n    \"RecallDate\": { \"type\": \"string\", \"format\": \"date\" },\n    \"Description\": { \"type\": \"string\" },\n    \"URL\": { \"type\": \"string\", \"format\": \"uri\" },\n    \"Title\": { \"type\": \"string\" },\n    \"ConsumerContact\": { \"type\": \"string\" },\n    \"LastPublishDate\": { \"type\": \"string\", \"format\": \"date\" },\n    \"Products\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"Name\": {\
  \ \"type\": \"string\" },\n          \"Description\": { \"type\": \"string\" },\n          \"Model\": { \"type\": \"string\" },\n          \"Type\": { \"type\": \"string\" },\n          \"CategoryID\": { \"type\": \"string\" },\n          \"NumberOfUnits\": { \"type\": \"string\" }\n        }\n      }\n    },\n    \"Inconjunctions\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": { \"Country\": { \"type\": \"string\" } }\n      }\n    },\n    \"Images\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"URL\": { \"type\": \"string\", \"format\": \"uri\" },\n          \"Caption\": { \"type\": \"string\" }\n        }\n      }\n    },\n    \"Injuries\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": { \"Name\": { \"type\": \"string\" } }\n      }\n    },\n    \"Manufacturers\": {\n      \"type\": \"array\"\
  ,\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"CompanyID\": { \"type\": \"integer\" },\n          \"Name\": { \"type\": \"string\" },\n          \"Country\": { \"type\": \"string\" }\n        }\n      }\n    },\n    \"Retailers\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": { \"Name\": { \"type\": \"string\" } }\n      }\n    },\n    \"Importers\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": { \"Name\": { \"type\": \"string\" } }\n      }\n    },\n    \"Distributors\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": { \"Name\": { \"type\": \"string\" } }\n      }\n    },\n    \"ManufacturerCountries\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": { \"Country\": { \"type\": \"string\" } }\n      }\n   \
  \ },\n    \"ProductUPCs\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": { \"UPC\": { \"type\": \"string\" } }\n      }\n    },\n    \"Hazards\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"Name\": { \"type\": \"string\" },\n          \"HazardType\": { \"type\": \"string\" },\n          \"HazardTypeID\": { \"type\": \"integer\" }\n        }\n      }\n    },\n    \"Remedies\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": { \"Name\": { \"type\": \"string\" } }\n      }\n    },\n    \"RemedyOptions\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": { \"Option\": { \"type\": \"string\" } }\n      }\n    }\n  },\n  \"required\": [\"RecallID\", \"RecallNumber\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/consumer-product-safety-commission/refs/heads/main/json-schema/cpsc-recall-schema.json
tags:
- Consumer Protection
- Federal Government
- Hazards
- Open Data
- Product Safety
- Recalls
title: CPSC Recall
---
