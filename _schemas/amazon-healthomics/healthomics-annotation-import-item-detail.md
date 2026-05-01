---
description: Details about an imported annotation item.
layout: schema
name: AnnotationImportItemDetail
properties_list:
- description: ''
  name: source
  type: object
- description: ''
  name: jobStatus
  type: object
provider_name: Amazon HealthOmics
provider_slug: amazon-healthomics
schema_file: json-schema/healthomics-annotation-import-item-detail-schema.json
slug: healthomics-annotation-import-item-detail
source_filename: healthomics-annotation-import-item-detail-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-healthomics/refs/heads/main/json-schema/healthomics-annotation-import-item-detail-schema.json\",\n  \"title\": \"AnnotationImportItemDetail\",\n  \"type\": \"object\",\n  \"required\": [\n    \"source\",\n    \"jobStatus\"\n  ],\n  \"properties\": {\n    \"source\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/S3Uri\"\n        },\n        {\n          \"description\": \"The source file's location in Amazon S3.\"\n        }\n      ]\n    },\n    \"jobStatus\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/JobStatus\"\n        },\n        {\n          \"description\": \"The item's job status.\"\n        }\n      ]\n    }\n  },\n  \"description\": \"Details about an imported annotation item.\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-healthomics/refs/heads/main/json-schema/healthomics-annotation-import-item-detail-schema.json
tags:
- Bioinformatics
- Genomics
- Healthcare
- Life Sciences
- Cloud Computing
title: AnnotationImportItemDetail
---
