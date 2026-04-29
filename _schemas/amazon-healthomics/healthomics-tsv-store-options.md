---
description: File settings for a TSV store.
layout: schema
name: TsvStoreOptions
properties_list:
- description: ''
  name: annotationType
  type: object
- description: ''
  name: formatToHeader
  type: object
- description: ''
  name: schema
  type: object
provider_name: Amazon HealthOmics
provider_slug: amazon-healthomics
schema_file: json-schema/healthomics-tsv-store-options-schema.json
slug: healthomics-tsv-store-options
source_filename: healthomics-tsv-store-options-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-healthomics/refs/heads/main/json-schema/healthomics-tsv-store-options-schema.json\",\n  \"title\": \"TsvStoreOptions\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"annotationType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AnnotationType\"\n        },\n        {\n          \"description\": \"The store's annotation type.\"\n        }\n      ]\n    },\n    \"formatToHeader\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FormatToHeader\"\n        },\n        {\n          \"description\": \"The store's header key to column name mapping.\"\n        }\n      ]\n    },\n    \"schema\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TsvStoreOptionsSchemaList\"\n        },\n        {\n          \"description\": \"The store's schema.\"\n     \
  \   }\n      ]\n    }\n  },\n  \"description\": \"File settings for a TSV store.\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-healthomics/refs/heads/main/json-schema/healthomics-tsv-store-options-schema.json
tags:
- AWS
- Bioinformatics
- Genomics
- Healthcare
- Life Sciences
- Cloud Computing
title: TsvStoreOptions
---
