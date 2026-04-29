---
description: Settings for a store.
layout: schema
name: StoreOptions
properties_list:
- description: ''
  name: tsvStoreOptions
  type: object
provider_name: Amazon HealthOmics
provider_slug: amazon-healthomics
schema_file: json-schema/healthomics-store-options-schema.json
slug: healthomics-store-options
source_filename: healthomics-store-options-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-healthomics/refs/heads/main/json-schema/healthomics-store-options-schema.json\",\n  \"title\": \"StoreOptions\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"tsvStoreOptions\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TsvStoreOptions\"\n        },\n        {\n          \"description\": \"File settings for a TSV store.\"\n        }\n      ]\n    }\n  },\n  \"description\": \"Settings for a store.\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-healthomics/refs/heads/main/json-schema/healthomics-store-options-schema.json
tags:
- AWS
- Bioinformatics
- Genomics
- Healthcare
- Life Sciences
- Cloud Computing
title: StoreOptions
---
