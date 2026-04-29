---
description: Acuity Brands product catalog item
layout: schema
name: CatalogItem
properties_list:
- description: Product number/SKU
  name: productNumber
  type: string
- description: Product name
  name: name
  type: string
- description: Brand name
  name: brand
  type: string
- description: Product category
  name: category
  type: string
- description: Product subcategory
  name: subcategory
  type: string
- description: Full product description
  name: description
  type: string
- description: Technical specifications
  name: specifications
  type: object
- description: Product certifications
  name: certifications
  type: array
- description: List price in USD
  name: listPrice
  type: number
- description: UPC code
  name: upc
  type: string
- description: Primary product image URL
  name: imageUrl
  type: string
- description: Product data sheet URL
  name: dataSheetUrl
  type: string
provider_name: acuity-brands
provider_slug: acuity-brands
schema_file: json-schema/acuity-brands-catalog-item-schema.json
slug: acuity-brands-catalog-item
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12\",\n  \"$id\": \"https://schema.api-evangelist.com/acuity-brands/acuity-brands-catalog-item-schema.json\",\n  \"title\": \"CatalogItem\",\n  \"description\": \"Acuity Brands product catalog item\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"productNumber\": {\n      \"type\": \"string\",\n      \"description\": \"Product number/SKU\",\n      \"example\": \"LBL4 48L ADP\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Product name\",\n      \"example\": \"4FT LED Wrap Light 4800 Lumens Adapter\"\n    },\n    \"brand\": {\n      \"type\": \"string\",\n      \"description\": \"Brand name\",\n      \"example\": \"Lithonia Lighting\"\n    },\n    \"category\": {\n      \"type\": \"string\",\n      \"description\": \"Product category\",\n      \"example\": \"Indoor Lighting\"\n    },\n    \"subcategory\": {\n      \"type\": \"string\",\n      \"description\": \"Product subcategory\"\
  ,\n      \"example\": \"Wrap Lights\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Full product description\"\n    },\n    \"specifications\": {\n      \"type\": \"object\",\n      \"description\": \"Technical specifications\",\n      \"additionalProperties\": true\n    },\n    \"certifications\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"Product certifications\",\n      \"example\": [\n        \"UL Listed\",\n        \"Energy Star\",\n        \"DLC Listed\"\n      ]\n    },\n    \"listPrice\": {\n      \"type\": \"number\",\n      \"description\": \"List price in USD\",\n      \"example\": 89.99\n    },\n    \"upc\": {\n      \"type\": \"string\",\n      \"description\": \"UPC code\",\n      \"example\": \"041194682000\"\n    },\n    \"imageUrl\": {\n      \"type\": \"string\",\n      \"description\": \"Primary product image URL\"\n    },\n    \"dataSheetUrl\": {\n     \
  \ \"type\": \"string\",\n      \"description\": \"Product data sheet URL\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/acuity-brands/refs/heads/main/json-schema/acuity-brands-catalog-item-schema.json
tags: []
title: CatalogItem
---
