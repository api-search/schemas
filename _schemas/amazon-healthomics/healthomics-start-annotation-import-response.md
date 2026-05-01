---
description: ''
layout: schema
name: StartAnnotationImportResponse
properties_list:
- description: ''
  name: jobId
  type: object
provider_name: Amazon HealthOmics
provider_slug: amazon-healthomics
schema_file: json-schema/healthomics-start-annotation-import-response-schema.json
slug: healthomics-start-annotation-import-response
source_filename: healthomics-start-annotation-import-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-healthomics/refs/heads/main/json-schema/healthomics-start-annotation-import-response-schema.json\",\n  \"title\": \"StartAnnotationImportResponse\",\n  \"type\": \"object\",\n  \"required\": [\n    \"jobId\"\n  ],\n  \"properties\": {\n    \"jobId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceId\"\n        },\n        {\n          \"description\": \"The job's ID.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-healthomics/refs/heads/main/json-schema/healthomics-start-annotation-import-response-schema.json
tags:
- Bioinformatics
- Genomics
- Healthcare
- Life Sciences
- Cloud Computing
title: StartAnnotationImportResponse
---
