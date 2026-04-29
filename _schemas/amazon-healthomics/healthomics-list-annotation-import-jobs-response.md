---
description: ''
layout: schema
name: ListAnnotationImportJobsResponse
properties_list:
- description: ''
  name: annotationImportJobs
  type: object
- description: ''
  name: nextToken
  type: object
provider_name: Amazon HealthOmics
provider_slug: amazon-healthomics
schema_file: json-schema/healthomics-list-annotation-import-jobs-response-schema.json
slug: healthomics-list-annotation-import-jobs-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-healthomics/refs/heads/main/json-schema/healthomics-list-annotation-import-jobs-response-schema.json\",\n  \"title\": \"ListAnnotationImportJobsResponse\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"annotationImportJobs\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AnnotationImportJobItems\"\n        },\n        {\n          \"description\": \"A list of jobs.\"\n        }\n      ]\n    },\n    \"nextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"A pagination token that's included if more results are available.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-healthomics/refs/heads/main/json-schema/healthomics-list-annotation-import-jobs-response-schema.json
tags:
- AWS
- Bioinformatics
- Genomics
- Healthcare
- Life Sciences
- Cloud Computing
title: ListAnnotationImportJobsResponse
---
