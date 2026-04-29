---
description: A subset of the possible batch job attributes. Used in the batch job list.
layout: schema
name: BatchJobExecutionSummary
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
  name: returnCode
  type: object
- description: ''
  name: startTime
  type: object
- description: ''
  name: status
  type: object
provider_name: Amazon Mainframe Modernization
provider_slug: amazon-mainframe-modernization
schema_file: json-schema/amazon-mainframe-modernization-batch-job-execution-summary-schema.json
slug: amazon-mainframe-modernization-batch-job-execution-summary
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mainframe-modernization/refs/heads/main/json-schema/amazon-mainframe-modernization-batch-job-execution-summary-schema.json\",\n  \"title\": \"BatchJobExecutionSummary\",\n  \"description\": \"A subset of the possible batch job attributes. Used in the batch job list.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"applicationId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Identifier\"\n        },\n        {\n          \"description\": \"The unique identifier of the application that hosts this batch job.\"\n        }\n      ]\n    },\n    \"batchJobIdentifier\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BatchJobIdentifier\"\n        },\n        {\n          \"description\": \"The unique identifier of this batch job.\"\n        }\n      ]\n    },\n    \"endTime\":\
  \ {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The timestamp when this batch job execution ended.\"\n        }\n      ]\n    },\n    \"executionId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Identifier\"\n        },\n        {\n          \"description\": \"The unique identifier of this execution of the batch job.\"\n        }\n      ]\n    },\n    \"jobId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String100\"\n        },\n        {\n          \"description\": \"The unique identifier of a particular batch job.\"\n        }\n      ]\n    },\n    \"jobName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String100\"\n        },\n        {\n          \"description\": \"The name of a particular batch job.\"\n        }\n      ]\n    },\n    \"jobType\": {\n      \"allOf\": [\n        {\n      \
  \    \"$ref\": \"#/components/schemas/BatchJobType\"\n        },\n        {\n          \"description\": \"The type of a particular batch job execution.\"\n        }\n      ]\n    },\n    \"returnCode\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The batch job return code from either the Blu Age or Micro Focus runtime engines. For more information, see <a href=\\\"https://www.ibm.com/docs/en/was/8.5.5?topic=model-batch-return-codes\\\">Batch return codes</a> in the <i>IBM WebSphere Application Server</i> documentation.\"\n        }\n      ]\n    },\n    \"startTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The timestamp when a particular batch job execution started.\"\n        }\n      ]\n    },\n    \"status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BatchJobExecutionStatus\"\
  \n        },\n        {\n          \"description\": \"The status of a particular batch job execution.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"applicationId\",\n    \"executionId\",\n    \"startTime\",\n    \"status\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mainframe-modernization/refs/heads/main/json-schema/amazon-mainframe-modernization-batch-job-execution-summary-schema.json
tags:
- AWS
- COBOL
- Mainframe
- Migration
- Modernization
- Batch Processing
title: BatchJobExecutionSummary
---
