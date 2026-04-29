---
description: A catalog item from a public catalog on SAP Business Network.
layout: schema
name: CatalogItem
properties_list:
- description: External product identifier.
  name: extProductId
  type: string
- description: Lead time in days.
  name: leadTime
  type: integer
- description: Manufacturer code.
  name: manufactCode
  type: string
- description: Manufacturer name.
  name: manufactName
  type: string
- description: Item price.
  name: price
  type: number
- description: Vendor identifier.
  name: vendor
  type: string
- description: Vendor display name.
  name: vendorName
  type: string
- description: Vendor-specific part identifier.
  name: vendorPartId
  type: string
provider_name: Ariba Guided Buying
provider_slug: ariba-guided-buying
schema_file: json-schema/catalog-shop-api-catalog-item-schema.json
slug: catalog-shop-api-catalog-item
source_filename: catalog-shop-api-catalog-item-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/ariba-guided-buying/refs/heads/main/json-schema/catalog-shop-api-catalog-item-schema.json\",\n  \"title\": \"CatalogItem\",\n  \"description\": \"A catalog item from a public catalog on SAP Business Network.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"extProductId\": {\n      \"type\": \"string\",\n      \"description\": \"External product identifier.\",\n      \"example\": \"PROD-001\"\n    },\n    \"leadTime\": {\n      \"type\": \"integer\",\n      \"description\": \"Lead time in days.\",\n      \"example\": 3\n    },\n    \"manufactCode\": {\n      \"type\": \"string\",\n      \"description\": \"Manufacturer code.\",\n      \"example\": \"MANUF-001\"\n    },\n    \"manufactName\": {\n      \"type\": \"string\",\n      \"description\": \"Manufacturer name.\",\n      \"example\": \"TechCorp\"\n    },\n    \"price\": {\n      \"type\"\
  : \"number\",\n      \"description\": \"Item price.\",\n      \"example\": 499.99\n    },\n    \"vendor\": {\n      \"type\": \"string\",\n      \"description\": \"Vendor identifier.\",\n      \"example\": \"VENDOR-A1B2\"\n    },\n    \"vendorName\": {\n      \"type\": \"string\",\n      \"description\": \"Vendor display name.\",\n      \"example\": \"Acme Office Supplies\"\n    },\n    \"vendorPartId\": {\n      \"type\": \"string\",\n      \"description\": \"Vendor-specific part identifier.\",\n      \"example\": \"AOS-LAPTOP-15\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/ariba-guided-buying/refs/heads/main/json-schema/catalog-shop-api-catalog-item-schema.json
tags:
- B2B
- Catalog
- ERP
- Procurement
- Requisitions
- SAP
- Supply Chain
title: CatalogItem
---
