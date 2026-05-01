---
description: ''
layout: schema
name: ListVariantStoresRequest
properties_list:
- description: ''
  name: ids
  type: object
- description: ''
  name: filter
  type: object
provider_name: Amazon HealthOmics
provider_slug: amazon-healthomics
schema_file: json-schema/healthomics-list-variant-stores-request-schema.json
slug: healthomics-list-variant-stores-request
source_filename: healthomics-list-variant-stores-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-healthomics/refs/heads/main/json-schema/healthomics-list-variant-stores-request-schema.json\",\n  \"title\": \"ListVariantStoresRequest\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ids\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ListVariantStoresRequestIdsList\"\n        },\n        {\n          \"description\": \"A list of store IDs.\"\n        }\n      ]\n    },\n    \"filter\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ListVariantStoresFilter\"\n        },\n        {\n          \"description\": \"A filter to apply to the list.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-healthomics/refs/heads/main/json-schema/healthomics-list-variant-stores-request-schema.json
tags:
- Bioinformatics
- Genomics
- Healthcare
- Life Sciences
- Cloud Computing
title: ListVariantStoresRequest
---
