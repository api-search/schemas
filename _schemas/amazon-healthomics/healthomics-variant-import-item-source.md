---
description: A imported variant item's source.
layout: schema
name: VariantImportItemSource
properties_list:
- description: ''
  name: source
  type: object
provider_name: Amazon HealthOmics
provider_slug: amazon-healthomics
schema_file: json-schema/healthomics-variant-import-item-source-schema.json
slug: healthomics-variant-import-item-source
source_filename: healthomics-variant-import-item-source-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-healthomics/refs/heads/main/json-schema/healthomics-variant-import-item-source-schema.json\",\n  \"title\": \"VariantImportItemSource\",\n  \"type\": \"object\",\n  \"required\": [\n    \"source\"\n  ],\n  \"properties\": {\n    \"source\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/S3Uri\"\n        },\n        {\n          \"description\": \"The source file's location in Amazon S3.\"\n        }\n      ]\n    }\n  },\n  \"description\": \"A imported variant item's source.\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-healthomics/refs/heads/main/json-schema/healthomics-variant-import-item-source-schema.json
tags:
- AWS
- Bioinformatics
- Genomics
- Healthcare
- Life Sciences
- Cloud Computing
title: VariantImportItemSource
---
