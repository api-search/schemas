---
description: GetExecutionHistoryInput schema from Amazon Step Functions API
layout: schema
name: GetExecutionHistoryInput
properties_list:
- description: ''
  name: executionArn
  type: object
- description: ''
  name: maxResults
  type: object
- description: ''
  name: reverseOrder
  type: object
- description: ''
  name: nextToken
  type: object
- description: ''
  name: includeExecutionData
  type: object
provider_name: Amazon Step Functions
provider_slug: amazon-step-functions
schema_file: json-schema/amazon-step-functions-get-execution-history-input-schema.json
slug: amazon-step-functions-get-execution-history-input
source_filename: amazon-step-functions-get-execution-history-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-step-functions/refs/heads/main/json-schema/amazon-step-functions-get-execution-history-input-schema.json\",\n  \"title\": \"GetExecutionHistoryInput\",\n  \"description\": \"GetExecutionHistoryInput schema from Amazon Step Functions API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"executionArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Arn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the execution.\"\n        }\n      ]\n    },\n    \"maxResults\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PageSize\"\n        },\n        {\n          \"description\": \"<p>The maximum number of results that are returned per call. You can use <code>nextToken</code> to obtain further pages of results. The default is 100 and the maximum\
  \ allowed page size is 1000. A value of 0 uses the default.</p> <p>This is only an upper limit. The actual number of results returned per call might be fewer than the specified maximum.</p>\"\n        }\n      ]\n    },\n    \"reverseOrder\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ReverseOrder\"\n        },\n        {\n          \"description\": \"Lists events in descending order of their <code>timeStamp</code>.\"\n        }\n      ]\n    },\n    \"nextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PageToken\"\n        },\n        {\n          \"description\": \"If <code>nextToken</code> is returned, there are more results available. The value of <code>nextToken</code> is a unique pagination token for each page. Make the call again using the returned token to retrieve the next page. Keep all other arguments unchanged. Each pagination token expires after 24 hours. Using an expired pagination token will return an\
  \ <i>HTTP 400 InvalidToken</i> error.\"\n        }\n      ]\n    },\n    \"includeExecutionData\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IncludeExecutionDataGetExecutionHistory\"\n        },\n        {\n          \"description\": \"You can select whether execution data (input or output of a history event) is returned. The default is <code>true</code>.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"executionArn\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-step-functions/refs/heads/main/json-schema/amazon-step-functions-get-execution-history-input-schema.json
tags:
- Orchestration
- Serverless
- State Machine
- Workflow
title: GetExecutionHistoryInput
---
