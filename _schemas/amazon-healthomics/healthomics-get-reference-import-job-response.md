---
description: ''
layout: schema
name: GetReferenceImportJobResponse
properties_list:
- description: ''
  name: id
  type: object
- description: ''
  name: referenceStoreId
  type: object
- description: ''
  name: roleArn
  type: object
- description: ''
  name: status
  type: object
- description: ''
  name: statusMessage
  type: object
- description: ''
  name: creationTime
  type: object
- description: ''
  name: completionTime
  type: object
- description: ''
  name: sources
  type: object
provider_name: Amazon HealthOmics
provider_slug: amazon-healthomics
schema_file: json-schema/healthomics-get-reference-import-job-response-schema.json
slug: healthomics-get-reference-import-job-response
source_filename: healthomics-get-reference-import-job-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-healthomics/refs/heads/main/json-schema/healthomics-get-reference-import-job-response-schema.json\",\n  \"title\": \"GetReferenceImportJobResponse\",\n  \"type\": \"object\",\n  \"required\": [\n    \"id\",\n    \"referenceStoreId\",\n    \"roleArn\",\n    \"status\",\n    \"creationTime\",\n    \"sources\"\n  ],\n  \"properties\": {\n    \"id\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ImportJobId\"\n        },\n        {\n          \"description\": \"The job's ID.\"\n        }\n      ]\n    },\n    \"referenceStoreId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ReferenceStoreId\"\n        },\n        {\n          \"description\": \"The job's reference store ID.\"\n        }\n      ]\n    },\n    \"roleArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RoleArn\"\
  \n        },\n        {\n          \"description\": \"The job's service role ARN.\"\n        }\n      ]\n    },\n    \"status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ReferenceImportJobStatus\"\n        },\n        {\n          \"description\": \"The job's status.\"\n        }\n      ]\n    },\n    \"statusMessage\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/JobStatusMessage\"\n        },\n        {\n          \"description\": \"The job's status message.\"\n        }\n      ]\n    },\n    \"creationTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SyntheticTimestamp_date_time\"\n        },\n        {\n          \"description\": \"When the job was created.\"\n        }\n      ]\n    },\n    \"completionTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SyntheticTimestamp_date_time\"\n        },\n        {\n          \"description\": \"When the job\
  \ completed.\"\n        }\n      ]\n    },\n    \"sources\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ImportReferenceSourceList\"\n        },\n        {\n          \"description\": \"The job's source files.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-healthomics/refs/heads/main/json-schema/healthomics-get-reference-import-job-response-schema.json
tags:
- Bioinformatics
- Genomics
- Healthcare
- Life Sciences
- Cloud Computing
title: GetReferenceImportJobResponse
---
