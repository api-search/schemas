---
description: ''
layout: schema
name: ListVariantStoresResponse
properties_list:
- description: ''
  name: variantStores
  type: object
- description: ''
  name: nextToken
  type: object
provider_name: Amazon HealthOmics
provider_slug: amazon-healthomics
schema_file: json-schema/healthomics-list-variant-stores-response-schema.json
slug: healthomics-list-variant-stores-response
source_filename: healthomics-list-variant-stores-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-healthomics/refs/heads/main/json-schema/healthomics-list-variant-stores-response-schema.json\",\n  \"title\": \"ListVariantStoresResponse\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"variantStores\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/VariantStoreItems\"\n        },\n        {\n          \"description\": \"A list of variant stores.\"\n        }\n      ]\n    },\n    \"nextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"A pagination token that's included if more results are available.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-healthomics/refs/heads/main/json-schema/healthomics-list-variant-stores-response-schema.json
tags:
- AWS
- Bioinformatics
- Genomics
- Healthcare
- Life Sciences
- Cloud Computing
title: ListVariantStoresResponse
---
