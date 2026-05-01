---
description: StartBatchJobRequest schema from AWS Mainframe Modernization API
layout: schema
name: StartBatchJobRequest
properties_list:
- description: ''
  name: batchJobIdentifier
  type: object
- description: ''
  name: jobParams
  type: object
provider_name: Amazon Mainframe Modernization
provider_slug: amazon-mainframe-modernization
schema_file: json-schema/amazon-mainframe-modernization-start-batch-job-request-schema.json
slug: amazon-mainframe-modernization-start-batch-job-request
source_filename: amazon-mainframe-modernization-start-batch-job-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mainframe-modernization/refs/heads/main/json-schema/amazon-mainframe-modernization-start-batch-job-request-schema.json\",\n  \"title\": \"StartBatchJobRequest\",\n  \"description\": \"StartBatchJobRequest schema from AWS Mainframe Modernization API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"batchJobIdentifier\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BatchJobIdentifier\"\n        },\n        {\n          \"description\": \"The unique identifier of the batch job.\"\n        }\n      ]\n    },\n    \"jobParams\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BatchJobParametersMap\"\n        },\n        {\n          \"description\": \"The collection of batch job parameters. For details about limits for keys and values, see <a href=\\\"https://www.ibm.com/docs/en/workload-automation/9.3.0?topic=zos-coding-variables-in-jcl\\\
  \">Coding variables in JCL</a>.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"batchJobIdentifier\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mainframe-modernization/refs/heads/main/json-schema/amazon-mainframe-modernization-start-batch-job-request-schema.json
tags:
- COBOL
- Mainframe
- Migration
- Modernization
- Batch Processing
title: StartBatchJobRequest
---
