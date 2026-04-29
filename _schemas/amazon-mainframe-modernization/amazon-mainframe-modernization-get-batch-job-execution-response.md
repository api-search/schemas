---
description: GetBatchJobExecutionResponse schema from AWS Mainframe Modernization API
layout: schema
name: GetBatchJobExecutionResponse
properties_list:
- description: ''
  name: applicationId
  type: object
- description: ''
  name: batchJobIdentifier
  type: object
- description: ''
  name: endTime
  type: object
- description: ''
  name: executionId
  type: object
- description: ''
  name: jobId
  type: object
- description: ''
  name: jobName
  type: object
- description: ''
  name: jobType
  type: object
- description: ''
  name: jobUser
  type: object
- description: ''
  name: returnCode
  type: object
- description: ''
  name: startTime
  type: object
- description: ''
  name: status
  type: object
- description: ''
  name: statusReason
  type: object
provider_name: Amazon Mainframe Modernization
provider_slug: amazon-mainframe-modernization
schema_file: json-schema/amazon-mainframe-modernization-get-batch-job-execution-response-schema.json
slug: amazon-mainframe-modernization-get-batch-job-execution-response
source_filename: amazon-mainframe-modernization-get-batch-job-execution-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mainframe-modernization/refs/heads/main/json-schema/amazon-mainframe-modernization-get-batch-job-execution-response-schema.json\",\n  \"title\": \"GetBatchJobExecutionResponse\",\n  \"description\": \"GetBatchJobExecutionResponse schema from AWS Mainframe Modernization API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"applicationId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Identifier\"\n        },\n        {\n          \"description\": \"The identifier of the application.\"\n        }\n      ]\n    },\n    \"batchJobIdentifier\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BatchJobIdentifier\"\n        },\n        {\n          \"description\": \"The unique identifier of this batch job.\"\n        }\n      ]\n    },\n    \"endTime\": {\n      \"allOf\": [\n  \
  \      {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The timestamp when the batch job execution ended.\"\n        }\n      ]\n    },\n    \"executionId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Identifier\"\n        },\n        {\n          \"description\": \"The unique identifier for this batch job execution.\"\n        }\n      ]\n    },\n    \"jobId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String100\"\n        },\n        {\n          \"description\": \"The unique identifier for this batch job.\"\n        }\n      ]\n    },\n    \"jobName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String100\"\n        },\n        {\n          \"description\": \"The name of this batch job.\"\n        }\n      ]\n    },\n    \"jobType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BatchJobType\"\
  \n        },\n        {\n          \"description\": \"The type of job.\"\n        }\n      ]\n    },\n    \"jobUser\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String100\"\n        },\n        {\n          \"description\": \"The user for the job.\"\n        }\n      ]\n    },\n    \"returnCode\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The batch job return code from either the Blu Age or Micro Focus runtime engines. For more information, see <a href=\\\"https://www.ibm.com/docs/en/was/8.5.5?topic=model-batch-return-codes\\\">Batch return codes</a> in the <i>IBM WebSphere Application Server</i> documentation.\"\n        }\n      ]\n    },\n    \"startTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The timestamp when the batch job execution started.\"\n \
  \       }\n      ]\n    },\n    \"status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BatchJobExecutionStatus\"\n        },\n        {\n          \"description\": \"The status of the batch job execution.\"\n        }\n      ]\n    },\n    \"statusReason\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The reason for the reported status.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"applicationId\",\n    \"executionId\",\n    \"startTime\",\n    \"status\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mainframe-modernization/refs/heads/main/json-schema/amazon-mainframe-modernization-get-batch-job-execution-response-schema.json
tags:
- AWS
- COBOL
- Mainframe
- Migration
- Modernization
- Batch Processing
title: GetBatchJobExecutionResponse
---
