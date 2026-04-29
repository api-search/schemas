---
description: ''
layout: schema
name: ListStateMachinesOutput
properties_list:
- description: ''
  name: stateMachines
  type: array
- description: ''
  name: nextToken
  type: object
provider_name: AWS Step Functions
provider_slug: aws-step-functions
schema_file: json-schema/step-functions-liststatemachinesoutput-schema.json
slug: step-functions-liststatemachinesoutput
source_filename: step-functions-liststatemachinesoutput-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ListStateMachinesOutput\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"stateMachines\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"stateMachineArn\": {\n            \"allOf\": [\n              {\n                \"$ref\": \"#/components/schemas/Arn\"\n              },\n              {\n                \"description\": \"The Amazon Resource Name (ARN) that identifies the state machine.\"\n              }\n            ]\n          },\n          \"name\": {\n            \"allOf\": [\n              {\n                \"$ref\": \"#/components/schemas/Name\"\n              },\n              {\n                \"description\": \"<p>The name of the state machine.</p> <p>A name must <i>not</i> contain:</p> <ul> <li> <p>white space</p> </li> <li> <p>brackets <code>&lt; &gt; { } [ ]</code> </p> </li> <li> <p>wildcard\
  \ characters <code>? *</code> </p> </li> <li> <p>special characters <code>\\\" # % \\\\ ^ | ~ ` $ &amp; , ; : /</code> </p> </li> <li> <p>control characters (<code>U+0000-001F</code>, <code>U+007F-009F</code>)</p> </li> </ul> <p>To enable logging with CloudWatch Logs, the name should only contain 0-9, A-Z, a-z, - and _.</p>\"\n              }\n            ]\n          },\n          \"type\": {\n            \"allOf\": [\n              {\n                \"$ref\": \"#/components/schemas/StateMachineType\"\n              },\n              {\n                \"description\": \"<p/>\"\n              }\n            ]\n          },\n          \"creationDate\": {\n            \"allOf\": [\n              {\n                \"$ref\": \"#/components/schemas/Timestamp\"\n              },\n              {\n                \"description\": \"The date the state machine is created.\"\n              }\n            ]\n          }\n        },\n        \"required\": [\n          \"stateMachineArn\",\n   \
  \       \"name\",\n          \"type\",\n          \"creationDate\"\n        ],\n        \"description\": \"Contains details about the state machine.\"\n      }\n    },\n    \"nextToken\": {}\n  },\n  \"required\": [\n    \"stateMachines\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-step-functions/refs/heads/main/json-schema/step-functions-liststatemachinesoutput-schema.json
tags:
- AWS
- iPaaS
- Orchestration
- Serverless
title: ListStateMachinesOutput
---
