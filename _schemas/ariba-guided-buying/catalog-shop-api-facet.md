---
description: A filter facet for catalog search results.
layout: schema
name: Facet
properties_list:
- description: Facet name.
  name: name
  type: string
- description: Facet values with counts.
  name: values
  type: array
provider_name: Ariba Guided Buying
provider_slug: ariba-guided-buying
schema_file: json-schema/catalog-shop-api-facet-schema.json
slug: catalog-shop-api-facet
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/ariba-guided-buying/refs/heads/main/json-schema/catalog-shop-api-facet-schema.json\",\n  \"title\": \"Facet\",\n  \"description\": \"A filter facet for catalog search results.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Facet name.\",\n      \"example\": \"Category\"\n    },\n    \"values\": {\n      \"type\": \"array\",\n      \"description\": \"Facet values with counts.\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/FacetValue\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/ariba-guided-buying/refs/heads/main/json-schema/catalog-shop-api-facet-schema.json
tags:
- B2B
- Catalog
- ERP
- Procurement
- Requisitions
- SAP
- Supply Chain
title: Facet
---
