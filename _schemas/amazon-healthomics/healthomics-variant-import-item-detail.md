---
description: Details about an imported variant item.
layout: schema
name: VariantImportItemDetail
properties_list:
- description: ''
  name: source
  type: object
- description: ''
  name: jobStatus
  type: object
- description: ''
  name: statusMessage
  type: object
provider_name: Amazon HealthOmics
provider_slug: amazon-healthomics
schema_file: json-schema/healthomics-variant-import-item-detail-schema.json
slug: healthomics-variant-import-item-detail
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-healthomics/refs/heads/main/json-schema/healthomics-variant-import-item-detail-schema.json\",\n  \"title\": \"VariantImportItemDetail\",\n  \"type\": \"object\",\n  \"required\": [\n    \"source\",\n    \"jobStatus\"\n  ],\n  \"properties\": {\n    \"source\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/S3Uri\"\n        },\n        {\n          \"description\": \"The source file's location in Amazon S3.\"\n        }\n      ]\n    },\n    \"jobStatus\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/JobStatus\"\n        },\n        {\n          \"description\": \"The item's job status.\"\n        }\n      ]\n    },\n    \"statusMessage\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/JobStatusMsg\"\n        },\n        {\n          \"description\"\
  : \" A message that provides additional context about a job \"\n        }\n      ]\n    }\n  },\n  \"description\": \"Details about an imported variant item.\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-healthomics/refs/heads/main/json-schema/healthomics-variant-import-item-detail-schema.json
tags:
- AWS
- Bioinformatics
- Genomics
- Healthcare
- Life Sciences
- Cloud Computing
title: VariantImportItemDetail
---
