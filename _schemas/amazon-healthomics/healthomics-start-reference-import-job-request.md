---
description: ''
layout: schema
name: StartReferenceImportJobRequest
properties_list:
- description: ''
  name: roleArn
  type: object
- description: ''
  name: clientToken
  type: object
- description: ''
  name: sources
  type: object
provider_name: Amazon HealthOmics
provider_slug: amazon-healthomics
schema_file: json-schema/healthomics-start-reference-import-job-request-schema.json
slug: healthomics-start-reference-import-job-request
source_filename: healthomics-start-reference-import-job-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-healthomics/refs/heads/main/json-schema/healthomics-start-reference-import-job-request-schema.json\",\n  \"title\": \"StartReferenceImportJobRequest\",\n  \"type\": \"object\",\n  \"required\": [\n    \"roleArn\",\n    \"sources\"\n  ],\n  \"properties\": {\n    \"roleArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RoleArn\"\n        },\n        {\n          \"description\": \"A service role for the job.\"\n        }\n      ]\n    },\n    \"clientToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ClientToken\"\n        },\n        {\n          \"description\": \"To ensure that jobs don't run multiple times, specify a unique token for each job.\"\n        }\n      ]\n    },\n    \"sources\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StartReferenceImportJobRequestSourcesList\"\
  \n        },\n        {\n          \"description\": \"The job's source files.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-healthomics/refs/heads/main/json-schema/healthomics-start-reference-import-job-request-schema.json
tags:
- Bioinformatics
- Genomics
- Healthcare
- Life Sciences
- Cloud Computing
title: StartReferenceImportJobRequest
---
