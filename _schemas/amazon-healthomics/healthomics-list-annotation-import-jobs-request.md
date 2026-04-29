---
description: ''
layout: schema
name: ListAnnotationImportJobsRequest
properties_list:
- description: ''
  name: ids
  type: object
- description: ''
  name: filter
  type: object
provider_name: Amazon HealthOmics
provider_slug: amazon-healthomics
schema_file: json-schema/healthomics-list-annotation-import-jobs-request-schema.json
slug: healthomics-list-annotation-import-jobs-request
source_filename: healthomics-list-annotation-import-jobs-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-healthomics/refs/heads/main/json-schema/healthomics-list-annotation-import-jobs-request-schema.json\",\n  \"title\": \"ListAnnotationImportJobsRequest\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ids\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ListAnnotationImportJobsRequestIdsList\"\n        },\n        {\n          \"description\": \"IDs of annotation import jobs to retrieve.\"\n        }\n      ]\n    },\n    \"filter\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ListAnnotationImportJobsFilter\"\n        },\n        {\n          \"description\": \"A filter to apply to the list.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-healthomics/refs/heads/main/json-schema/healthomics-list-annotation-import-jobs-request-schema.json
tags:
- AWS
- Bioinformatics
- Genomics
- Healthcare
- Life Sciences
- Cloud Computing
title: ListAnnotationImportJobsRequest
---
