---
description: Contains details about an execution.
layout: schema
name: ExecutionListItem
properties_list:
- description: ''
  name: executionArn
  type: object
- description: ''
  name: stateMachineArn
  type: object
- description: ''
  name: name
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
  name: mapRunArn
  type: object
- description: ''
  name: itemCount
  type: object
- description: ''
  name: stateMachineVersionArn
  type: object
- description: ''
  name: stateMachineAliasArn
  type: object
provider_name: Amazon Step Functions
provider_slug: amazon-step-functions
schema_file: json-schema/amazon-step-functions-execution-list-item-schema.json
slug: amazon-step-functions-execution-list-item
source_filename: amazon-step-functions-execution-list-item-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-step-functions/refs/heads/main/json-schema/amazon-step-functions-execution-list-item-schema.json\",\n  \"title\": \"ExecutionListItem\",\n  \"description\": \"Contains details about an execution.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"executionArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Arn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) that identifies the execution.\"\n        }\n      ]\n    },\n    \"stateMachineArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Arn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the state machine that ran the execution.\"\n        }\n      ]\n    },\n    \"name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Name\"\
  \n        },\n        {\n          \"description\": \"<p>The name of the execution.</p> <p>A name must <i>not</i> contain:</p> <ul> <li> <p>white space</p> </li> <li> <p>brackets <code>&lt; &gt; { } [ ]</code> </p> </li> <li> <p>wildcard characters <code>? *</code> </p> </li> <li> <p>special characters <code>\\\" # % \\\\ ^ | ~ ` $ &amp; , ; : /</code> </p> </li> <li> <p>control characters (<code>U+0000-001F</code>, <code>U+007F-009F</code>)</p> </li> </ul> <p>To enable logging with CloudWatch Logs, the name should only contain 0-9, A-Z, a-z, - and _.</p>\"\n        }\n      ]\n    },\n    \"status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ExecutionStatus\"\n        },\n        {\n          \"description\": \"The current status of the execution.\"\n        }\n      ]\n    },\n    \"startDate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The date the execution\
  \ started.\"\n        }\n      ]\n    },\n    \"stopDate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"If the execution already ended, the date the execution stopped.\"\n        }\n      ]\n    },\n    \"mapRunArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LongArn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of a Map Run. This field is returned only if <code>mapRunArn</code> was specified in the <code>ListExecutions</code> API action. If <code>stateMachineArn</code> was specified in <code>ListExecutions</code>, the <code>mapRunArn</code> isn't returned.\"\n        }\n      ]\n    },\n    \"itemCount\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UnsignedInteger\"\n        },\n        {\n          \"description\": \"The total number of items processed in a child workflow execution.\
  \ This field is returned only if <code>mapRunArn</code> was specified in the <code>ListExecutions</code> API action. If <code>stateMachineArn</code> was specified in <code>ListExecutions</code>, the <code>itemCount</code> field isn't returned.\"\n        }\n      ]\n    },\n    \"stateMachineVersionArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Arn\"\n        },\n        {\n          \"description\": \"<p>The Amazon Resource Name (ARN) of the state machine version associated with the execution.</p> <p>If the state machine execution was started with an unqualified ARN, it returns null.</p> <p>If the execution was started using a <code>stateMachineAliasArn</code>, both the <code>stateMachineAliasArn</code> and <code>stateMachineVersionArn</code> parameters contain the respective values.</p>\"\n        }\n      ]\n    },\n    \"stateMachineAliasArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Arn\"\n        },\n     \
  \   {\n          \"description\": \"<p>The Amazon Resource Name (ARN) of the state machine alias used to start an execution.</p> <p>If the state machine execution was started with an unqualified ARN or a version ARN, it returns null.</p>\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"executionArn\",\n    \"stateMachineArn\",\n    \"name\",\n    \"status\",\n    \"startDate\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-step-functions/refs/heads/main/json-schema/amazon-step-functions-execution-list-item-schema.json
tags:
- Orchestration
- Serverless
- State Machine
- Workflow
title: ExecutionListItem
---
