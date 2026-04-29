---
description: Response containing a list of catalog items.
layout: schema
name: ItemsResponse
properties_list:
- description: List of catalog items.
  name: items
  type: array
provider_name: Ariba Guided Buying
provider_slug: ariba-guided-buying
schema_file: json-schema/catalog-shop-api-items-response-schema.json
slug: catalog-shop-api-items-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/ariba-guided-buying/refs/heads/main/json-schema/catalog-shop-api-items-response-schema.json\",\n  \"title\": \"ItemsResponse\",\n  \"description\": \"Response containing a list of catalog items.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"items\": {\n      \"type\": \"array\",\n      \"description\": \"List of catalog items.\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/CatalogItem\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/ariba-guided-buying/refs/heads/main/json-schema/catalog-shop-api-items-response-schema.json
tags:
- B2B
- Catalog
- ERP
- Procurement
- Requisitions
- SAP
- Supply Chain
title: ItemsResponse
---
