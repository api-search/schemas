---
description: Response containing catalog items and facets for a shop.
layout: schema
name: ShopResponse
properties_list:
- description: The unique identifier of the shop.
  name: shopID
  type: string
- description: List of catalog items.
  name: items
  type: array
- description: List of filter facets.
  name: facets
  type: array
provider_name: Ariba Guided Buying
provider_slug: ariba-guided-buying
schema_file: json-schema/catalog-shop-api-shop-response-schema.json
slug: catalog-shop-api-shop-response
source_filename: catalog-shop-api-shop-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/ariba-guided-buying/refs/heads/main/json-schema/catalog-shop-api-shop-response-schema.json\",\n  \"title\": \"ShopResponse\",\n  \"description\": \"Response containing catalog items and facets for a shop.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"shopID\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier of the shop.\",\n      \"example\": \"shop-12345\"\n    },\n    \"items\": {\n      \"type\": \"array\",\n      \"description\": \"List of catalog items.\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/CatalogItem\"\n      }\n    },\n    \"facets\": {\n      \"type\": \"array\",\n      \"description\": \"List of filter facets.\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/Facet\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/ariba-guided-buying/refs/heads/main/json-schema/catalog-shop-api-shop-response-schema.json
tags:
- B2B
- Catalog
- ERP
- Procurement
- Requisitions
- SAP
- Supply Chain
title: ShopResponse
---
