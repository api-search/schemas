---
description: ''
layout: schema
name: StartReadSetImportJobResponse
properties_list:
- description: ''
  name: id
  type: object
- description: ''
  name: sequenceStoreId
  type: object
- description: ''
  name: roleArn
  type: object
- description: ''
  name: status
  type: object
- description: ''
  name: creationTime
  type: object
provider_name: Amazon HealthOmics
provider_slug: amazon-healthomics
schema_file: json-schema/healthomics-start-read-set-import-job-response-schema.json
slug: healthomics-start-read-set-import-job-response
source_filename: healthomics-start-read-set-import-job-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-healthomics/refs/heads/main/json-schema/healthomics-start-read-set-import-job-response-schema.json\",\n  \"title\": \"StartReadSetImportJobResponse\",\n  \"type\": \"object\",\n  \"required\": [\n    \"id\",\n    \"sequenceStoreId\",\n    \"roleArn\",\n    \"status\",\n    \"creationTime\"\n  ],\n  \"properties\": {\n    \"id\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ImportJobId\"\n        },\n        {\n          \"description\": \"The job's ID.\"\n        }\n      ]\n    },\n    \"sequenceStoreId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SequenceStoreId\"\n        },\n        {\n          \"description\": \"The read set's sequence store ID.\"\n        }\n      ]\n    },\n    \"roleArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RoleArn\"\
  \n        },\n        {\n          \"description\": \"The job's service role ARN.\"\n        }\n      ]\n    },\n    \"status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ReadSetImportJobStatus\"\n        },\n        {\n          \"description\": \"The job's status.\"\n        }\n      ]\n    },\n    \"creationTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SyntheticTimestamp_date_time\"\n        },\n        {\n          \"description\": \"When the job was created.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-healthomics/refs/heads/main/json-schema/healthomics-start-read-set-import-job-response-schema.json
tags:
- Bioinformatics
- Genomics
- Healthcare
- Life Sciences
- Cloud Computing
title: StartReadSetImportJobResponse
---
