---
description: ''
layout: schema
name: BatchDeleteReadSetRequest
properties_list:
- description: ''
  name: ids
  type: object
provider_name: Amazon HealthOmics
provider_slug: amazon-healthomics
schema_file: json-schema/healthomics-batch-delete-read-set-request-schema.json
slug: healthomics-batch-delete-read-set-request
source_filename: healthomics-batch-delete-read-set-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-healthomics/refs/heads/main/json-schema/healthomics-batch-delete-read-set-request-schema.json\",\n  \"title\": \"BatchDeleteReadSetRequest\",\n  \"type\": \"object\",\n  \"required\": [\n    \"ids\"\n  ],\n  \"properties\": {\n    \"ids\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ReadSetIdList\"\n        },\n        {\n          \"description\": \"The read sets' IDs.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-healthomics/refs/heads/main/json-schema/healthomics-batch-delete-read-set-request-schema.json
tags:
- AWS
- Bioinformatics
- Genomics
- Healthcare
- Life Sciences
- Cloud Computing
title: BatchDeleteReadSetRequest
---
