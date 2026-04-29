---
description: A source for an annotation import job.
layout: schema
name: AnnotationImportItemSource
properties_list:
- description: ''
  name: source
  type: object
provider_name: Amazon HealthOmics
provider_slug: amazon-healthomics
schema_file: json-schema/healthomics-annotation-import-item-source-schema.json
slug: healthomics-annotation-import-item-source
source_filename: healthomics-annotation-import-item-source-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-healthomics/refs/heads/main/json-schema/healthomics-annotation-import-item-source-schema.json\",\n  \"title\": \"AnnotationImportItemSource\",\n  \"type\": \"object\",\n  \"required\": [\n    \"source\"\n  ],\n  \"properties\": {\n    \"source\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/S3Uri\"\n        },\n        {\n          \"description\": \"The source file's location in Amazon S3.\"\n        }\n      ]\n    }\n  },\n  \"description\": \"A source for an annotation import job.\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-healthomics/refs/heads/main/json-schema/healthomics-annotation-import-item-source-schema.json
tags:
- AWS
- Bioinformatics
- Genomics
- Healthcare
- Life Sciences
- Cloud Computing
title: AnnotationImportItemSource
---
