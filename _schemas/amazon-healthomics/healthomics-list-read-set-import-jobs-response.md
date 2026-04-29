---
description: ''
layout: schema
name: ListReadSetImportJobsResponse
properties_list:
- description: ''
  name: nextToken
  type: object
- description: ''
  name: importJobs
  type: object
provider_name: Amazon HealthOmics
provider_slug: amazon-healthomics
schema_file: json-schema/healthomics-list-read-set-import-jobs-response-schema.json
slug: healthomics-list-read-set-import-jobs-response
source_filename: healthomics-list-read-set-import-jobs-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-healthomics/refs/heads/main/json-schema/healthomics-list-read-set-import-jobs-response-schema.json\",\n  \"title\": \"ListReadSetImportJobsResponse\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"nextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NextToken\"\n        },\n        {\n          \"description\": \"A pagination token that's included if more results are available.\"\n        }\n      ]\n    },\n    \"importJobs\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ImportReadSetJobList\"\n        },\n        {\n          \"description\": \"A list of jobs.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-healthomics/refs/heads/main/json-schema/healthomics-list-read-set-import-jobs-response-schema.json
tags:
- AWS
- Bioinformatics
- Genomics
- Healthcare
- Life Sciences
- Cloud Computing
title: ListReadSetImportJobsResponse
---
