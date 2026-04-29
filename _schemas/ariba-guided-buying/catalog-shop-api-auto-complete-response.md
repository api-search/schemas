---
description: Response containing typeahead search suggestions.
layout: schema
name: AutoCompleteResponse
properties_list:
- description: List of matching search suggestion strings.
  name: suggestions
  type: array
provider_name: Ariba Guided Buying
provider_slug: ariba-guided-buying
schema_file: json-schema/catalog-shop-api-auto-complete-response-schema.json
slug: catalog-shop-api-auto-complete-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/ariba-guided-buying/refs/heads/main/json-schema/catalog-shop-api-auto-complete-response-schema.json\",\n  \"title\": \"AutoCompleteResponse\",\n  \"description\": \"Response containing typeahead search suggestions.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"suggestions\": {\n      \"type\": \"array\",\n      \"description\": \"List of matching search suggestion strings.\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"example\": [\n        \"laptop\",\n        \"laptop stand\"\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/ariba-guided-buying/refs/heads/main/json-schema/catalog-shop-api-auto-complete-response-schema.json
tags:
- B2B
- Catalog
- ERP
- Procurement
- Requisitions
- SAP
- Supply Chain
title: AutoCompleteResponse
---
