---
description: ''
layout: schema
name: BatchDeleteReadSetResponse
properties_list:
- description: ''
  name: errors
  type: object
provider_name: Amazon HealthOmics
provider_slug: amazon-healthomics
schema_file: json-schema/healthomics-batch-delete-read-set-response-schema.json
slug: healthomics-batch-delete-read-set-response
source_filename: healthomics-batch-delete-read-set-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-healthomics/refs/heads/main/json-schema/healthomics-batch-delete-read-set-response-schema.json\",\n  \"title\": \"BatchDeleteReadSetResponse\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"errors\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ReadSetBatchErrorList\"\n        },\n        {\n          \"description\": \"Errors returned by individual delete operations.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-healthomics/refs/heads/main/json-schema/healthomics-batch-delete-read-set-response-schema.json
tags:
- Bioinformatics
- Genomics
- Healthcare
- Life Sciences
- Cloud Computing
title: BatchDeleteReadSetResponse
---
