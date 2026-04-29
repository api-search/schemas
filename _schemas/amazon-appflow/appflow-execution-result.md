---
description: ExecutionResult schema from Amazon AppFlow API
layout: schema
name: ExecutionResult
properties_list:
- description: Provides any error message information related to the flow run.
  name: errorInfo
  type: object
- description: The total number of bytes processed by the flow run.
  name: bytesProcessed
  type: integer
- description: The total number of bytes written as a result of the flow run.
  name: bytesWritten
  type: integer
- description: The number of records processed in the flow run.
  name: recordsProcessed
  type: integer
- description: The number of processes that Amazon AppFlow ran at the same time when it retrieved your data.
  name: numParallelProcesses
  type: integer
provider_name: Amazon AppFlow
provider_slug: amazon-appflow
schema_file: json-schema/appflow-execution-result-schema.json
slug: appflow-execution-result
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-appflow/refs/heads/main/json-schema/appflow-execution-result-schema.json\",\n  \"title\": \"ExecutionResult\",\n  \"description\": \"ExecutionResult schema from Amazon AppFlow API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"errorInfo\": {\n      \"type\": \"object\",\n      \"description\": \"Provides any error message information related to the flow run.\"\n    },\n    \"bytesProcessed\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\",\n      \"example\": 204800,\n      \"description\": \"The total number of bytes processed by the flow run.\"\n    },\n    \"bytesWritten\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\",\n      \"example\": 204800,\n      \"description\": \"The total number of bytes written as a result of the flow run.\"\n    },\n    \"recordsProcessed\": {\n      \"type\": \"integer\"\
  ,\n      \"format\": \"int64\",\n      \"example\": 1500,\n      \"description\": \"The number of records processed in the flow run.\"\n    },\n    \"numParallelProcesses\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\",\n      \"example\": 1,\n      \"description\": \"The number of processes that Amazon AppFlow ran at the same time when it retrieved your data.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-appflow/refs/heads/main/json-schema/appflow-execution-result-schema.json
tags:
- AWS
- Connectors
- Data Flow
- Data Integration
- ETL
- Integration
- SaaS
- Data Transfer
title: ExecutionResult
---
