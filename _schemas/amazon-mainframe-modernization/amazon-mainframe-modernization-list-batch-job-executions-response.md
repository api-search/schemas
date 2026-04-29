---
description: ListBatchJobExecutionsResponse schema from AWS Mainframe Modernization API
layout: schema
name: ListBatchJobExecutionsResponse
properties_list:
- description: ''
  name: batchJobExecutions
  type: object
- description: ''
  name: nextToken
  type: object
provider_name: Amazon Mainframe Modernization
provider_slug: amazon-mainframe-modernization
schema_file: json-schema/amazon-mainframe-modernization-list-batch-job-executions-response-schema.json
slug: amazon-mainframe-modernization-list-batch-job-executions-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mainframe-modernization/refs/heads/main/json-schema/amazon-mainframe-modernization-list-batch-job-executions-response-schema.json\",\n  \"title\": \"ListBatchJobExecutionsResponse\",\n  \"description\": \"ListBatchJobExecutionsResponse schema from AWS Mainframe Modernization API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"batchJobExecutions\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BatchJobExecutionSummaryList\"\n        },\n        {\n          \"description\": \"Returns a list of batch job executions for an application.\"\n        }\n      ]\n    },\n    \"nextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NextToken\"\n        },\n        {\n          \"description\": \"A pagination token that's returned when the response doesn't contain all batch job\
  \ executions.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"batchJobExecutions\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mainframe-modernization/refs/heads/main/json-schema/amazon-mainframe-modernization-list-batch-job-executions-response-schema.json
tags:
- AWS
- COBOL
- Mainframe
- Migration
- Modernization
- Batch Processing
title: ListBatchJobExecutionsResponse
---
