---
description: DescribeMapRunOutput schema from Amazon Step Functions API
layout: schema
name: DescribeMapRunOutput
properties_list:
- description: ''
  name: mapRunArn
  type: object
- description: ''
  name: executionArn
  type: object
- description: ''
  name: status
  type: object
- description: ''
  name: startDate
  type: object
- description: ''
  name: stopDate
  type: object
- description: ''
  name: maxConcurrency
  type: object
- description: ''
  name: toleratedFailurePercentage
  type: object
- description: ''
  name: toleratedFailureCount
  type: object
- description: ''
  name: itemCounts
  type: object
- description: ''
  name: executionCounts
  type: object
provider_name: Amazon Step Functions
provider_slug: amazon-step-functions
schema_file: json-schema/amazon-step-functions-describe-map-run-output-schema.json
slug: amazon-step-functions-describe-map-run-output
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-step-functions/refs/heads/main/json-schema/amazon-step-functions-describe-map-run-output-schema.json\",\n  \"title\": \"DescribeMapRunOutput\",\n  \"description\": \"DescribeMapRunOutput schema from Amazon Step Functions API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"mapRunArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LongArn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) that identifies a Map Run.\"\n        }\n      ]\n    },\n    \"executionArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Arn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) that identifies the execution in which the Map Run was started.\"\n        }\n      ]\n    },\n    \"status\": {\n      \"allOf\": [\n   \
  \     {\n          \"$ref\": \"#/components/schemas/MapRunStatus\"\n        },\n        {\n          \"description\": \"The current status of the Map Run.\"\n        }\n      ]\n    },\n    \"startDate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The date when the Map Run was started.\"\n        }\n      ]\n    },\n    \"stopDate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The date when the Map Run was stopped.\"\n        }\n      ]\n    },\n    \"maxConcurrency\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MaxConcurrency\"\n        },\n        {\n          \"description\": \"The maximum number of child workflow executions configured to run in parallel for the Map Run at the same time.\"\n        }\n      ]\n    },\n    \"toleratedFailurePercentage\": {\n\
  \      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ToleratedFailurePercentage\"\n        },\n        {\n          \"description\": \"The maximum percentage of failed child workflow executions before the Map Run fails.\"\n        }\n      ]\n    },\n    \"toleratedFailureCount\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ToleratedFailureCount\"\n        },\n        {\n          \"description\": \"The maximum number of failed child workflow executions before the Map Run fails.\"\n        }\n      ]\n    },\n    \"itemCounts\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MapRunItemCounts\"\n        },\n        {\n          \"description\": \"A JSON object that contains information about the total number of items, and the item count for each processing status, such as <code>pending</code> and <code>failed</code>.\"\n        }\n      ]\n    },\n    \"executionCounts\": {\n      \"allOf\": [\n       \
  \ {\n          \"$ref\": \"#/components/schemas/MapRunExecutionCounts\"\n        },\n        {\n          \"description\": \"A JSON object that contains information about the total number of child workflow executions for the Map Run, and the count of child workflow executions for each status, such as <code>failed</code> and <code>succeeded</code>.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"mapRunArn\",\n    \"executionArn\",\n    \"status\",\n    \"startDate\",\n    \"maxConcurrency\",\n    \"toleratedFailurePercentage\",\n    \"toleratedFailureCount\",\n    \"itemCounts\",\n    \"executionCounts\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-step-functions/refs/heads/main/json-schema/amazon-step-functions-describe-map-run-output-schema.json
tags:
- AWS
- Orchestration
- Serverless
- State Machine
- Workflow
title: DescribeMapRunOutput
---
