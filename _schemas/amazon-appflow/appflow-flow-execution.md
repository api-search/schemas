---
description: FlowExecution schema from Amazon AppFlow API
layout: schema
name: FlowExecution
properties_list:
- description: Specifies the identifier of the given flow run.
  name: executionId
  type: string
- description: Specifies the flow run status and whether it is in progress, has completed successfully, or has failed.
  name: executionStatus
  type: string
- description: ''
  name: executionResult
  type: object
- description: Specifies the start timestamp for your flow run.
  name: startedAt
  type: integer
- description: Specifies the time of the most recent update.
  name: lastUpdatedAt
  type: integer
- description: The timestamp that determines the first new or updated record to be transferred in the flow run.
  name: dataPullStartTime
  type: integer
- description: The timestamp that determines the last new or updated record to be transferred in the flow run.
  name: dataPullEndTime
  type: integer
provider_name: Amazon AppFlow
provider_slug: amazon-appflow
schema_file: json-schema/appflow-flow-execution-schema.json
slug: appflow-flow-execution
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-appflow/refs/heads/main/json-schema/appflow-flow-execution-schema.json\",\n  \"title\": \"FlowExecution\",\n  \"description\": \"FlowExecution schema from Amazon AppFlow API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"executionId\": {\n      \"type\": \"string\",\n      \"example\": \"exec-500123\",\n      \"description\": \"Specifies the identifier of the given flow run.\"\n    },\n    \"executionStatus\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"InProgress\",\n        \"Successful\",\n        \"Error\",\n        \"CancelStarted\",\n        \"Canceled\"\n      ],\n      \"example\": \"Successful\",\n      \"description\": \"Specifies the flow run status and whether it is in progress, has completed successfully, or has failed.\"\n    },\n    \"executionResult\": {\n      \"type\": \"object\",\n      \"properties\"\
  : {\n        \"errorInfo\": {\n          \"type\": \"object\",\n          \"description\": \"Provides any error message information related to the flow run.\"\n        },\n        \"bytesProcessed\": {\n          \"type\": \"integer\",\n          \"format\": \"int64\",\n          \"example\": 204800,\n          \"description\": \"The total number of bytes processed by the flow run.\"\n        },\n        \"bytesWritten\": {\n          \"type\": \"integer\",\n          \"format\": \"int64\",\n          \"example\": 204800,\n          \"description\": \"The total number of bytes written as a result of the flow run.\"\n        },\n        \"recordsProcessed\": {\n          \"type\": \"integer\",\n          \"format\": \"int64\",\n          \"example\": 1500,\n          \"description\": \"The number of records processed in the flow run.\"\n        },\n        \"numParallelProcesses\": {\n          \"type\": \"integer\",\n          \"format\": \"int64\",\n          \"example\": 1,\n       \
  \   \"description\": \"The number of processes that Amazon AppFlow ran at the same time when it retrieved your data.\"\n        }\n      }\n    },\n    \"startedAt\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\",\n      \"example\": 1718153645993,\n      \"description\": \"Specifies the start timestamp for your flow run.\"\n    },\n    \"lastUpdatedAt\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\",\n      \"example\": 1718153700000,\n      \"description\": \"Specifies the time of the most recent update.\"\n    },\n    \"dataPullStartTime\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\",\n      \"example\": 1718153645993,\n      \"description\": \"The timestamp that determines the first new or updated record to be transferred in the flow run.\"\n    },\n    \"dataPullEndTime\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\",\n      \"example\": 1718153700000,\n      \"description\": \"The timestamp that determines the last new\
  \ or updated record to be transferred in the flow run.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-appflow/refs/heads/main/json-schema/appflow-flow-execution-schema.json
tags:
- AWS
- Connectors
- Data Flow
- Data Integration
- ETL
- Integration
- SaaS
- Data Transfer
title: FlowExecution
---
