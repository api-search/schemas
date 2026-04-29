---
description: A filter for annotation import jobs.
layout: schema
name: ListAnnotationImportJobsFilter
properties_list:
- description: ''
  name: status
  type: object
- description: ''
  name: storeName
  type: object
provider_name: Amazon HealthOmics
provider_slug: amazon-healthomics
schema_file: json-schema/healthomics-list-annotation-import-jobs-filter-schema.json
slug: healthomics-list-annotation-import-jobs-filter
source_filename: healthomics-list-annotation-import-jobs-filter-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-healthomics/refs/heads/main/json-schema/healthomics-list-annotation-import-jobs-filter-schema.json\",\n  \"title\": \"ListAnnotationImportJobsFilter\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/JobStatus\"\n        },\n        {\n          \"description\": \"A status to filter on.\"\n        }\n      ]\n    },\n    \"storeName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"A store name to filter on.\"\n        }\n      ]\n    }\n  },\n  \"description\": \"A filter for annotation import jobs.\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-healthomics/refs/heads/main/json-schema/healthomics-list-annotation-import-jobs-filter-schema.json
tags:
- AWS
- Bioinformatics
- Genomics
- Healthcare
- Life Sciences
- Cloud Computing
title: ListAnnotationImportJobsFilter
---
