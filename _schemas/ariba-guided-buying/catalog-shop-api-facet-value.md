---
description: A single facet value with item count.
layout: schema
name: FacetValue
properties_list:
- description: Display label for this facet value.
  name: label
  type: string
- description: Number of items matching this facet value.
  name: count
  type: integer
provider_name: Ariba Guided Buying
provider_slug: ariba-guided-buying
schema_file: json-schema/catalog-shop-api-facet-value-schema.json
slug: catalog-shop-api-facet-value
source_filename: catalog-shop-api-facet-value-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/ariba-guided-buying/refs/heads/main/json-schema/catalog-shop-api-facet-value-schema.json\",\n  \"title\": \"FacetValue\",\n  \"description\": \"A single facet value with item count.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"label\": {\n      \"type\": \"string\",\n      \"description\": \"Display label for this facet value.\",\n      \"example\": \"Electronics\"\n    },\n    \"count\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of items matching this facet value.\",\n      \"example\": 42\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/ariba-guided-buying/refs/heads/main/json-schema/catalog-shop-api-facet-value-schema.json
tags:
- B2B
- Catalog
- ERP
- Procurement
- Requisitions
- SAP
- Supply Chain
title: FacetValue
---
