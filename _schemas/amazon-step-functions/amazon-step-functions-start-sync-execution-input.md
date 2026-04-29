---
description: StartSyncExecutionInput schema from Amazon Step Functions API
layout: schema
name: StartSyncExecutionInput
properties_list:
- description: ''
  name: stateMachineArn
  type: object
- description: ''
  name: name
  type: object
- description: ''
  name: input
  type: object
- description: ''
  name: traceHeader
  type: object
provider_name: Amazon Step Functions
provider_slug: amazon-step-functions
schema_file: json-schema/amazon-step-functions-start-sync-execution-input-schema.json
slug: amazon-step-functions-start-sync-execution-input
source_filename: amazon-step-functions-start-sync-execution-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-step-functions/refs/heads/main/json-schema/amazon-step-functions-start-sync-execution-input-schema.json\",\n  \"title\": \"StartSyncExecutionInput\",\n  \"description\": \"StartSyncExecutionInput schema from Amazon Step Functions API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"stateMachineArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Arn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the state machine to execute.\"\n        }\n      ]\n    },\n    \"name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Name\"\n        },\n        {\n          \"description\": \"The name of the execution.\"\n        }\n      ]\n    },\n    \"input\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SensitiveData\"\
  \n        },\n        {\n          \"description\": \"<p>The string that contains the JSON input data for the execution, for example:</p> <p> <code>\\\"input\\\": \\\"{\\\\\\\"first_name\\\\\\\" : \\\\\\\"test\\\\\\\"}\\\"</code> </p> <note> <p>If you don't include any JSON input data, you still must include the two braces, for example: <code>\\\"input\\\": \\\"{}\\\"</code> </p> </note> <p>Length constraints apply to the payload size, and are expressed as bytes in UTF-8 encoding.</p>\"\n        }\n      ]\n    },\n    \"traceHeader\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TraceHeader\"\n        },\n        {\n          \"description\": \"Passes the X-Ray trace header. The trace header can also be passed in the request payload.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"stateMachineArn\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-step-functions/refs/heads/main/json-schema/amazon-step-functions-start-sync-execution-input-schema.json
tags:
- AWS
- Orchestration
- Serverless
- State Machine
- Workflow
title: StartSyncExecutionInput
---
