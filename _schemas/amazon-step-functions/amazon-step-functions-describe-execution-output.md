---
description: DescribeExecutionOutput schema from Amazon Step Functions API
layout: schema
name: DescribeExecutionOutput
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
  name: input
  type: object
- description: ''
  name: inputDetails
  type: object
- description: ''
  name: output
  type: object
- description: ''
  name: outputDetails
  type: object
- description: ''
  name: traceHeader
  type: object
- description: ''
  name: mapRunArn
  type: object
- description: ''
  name: error
  type: object
- description: ''
  name: cause
  type: object
- description: ''
  name: stateMachineVersionArn
  type: object
- description: ''
  name: stateMachineAliasArn
  type: object
provider_name: Amazon Step Functions
provider_slug: amazon-step-functions
schema_file: json-schema/amazon-step-functions-describe-execution-output-schema.json
slug: amazon-step-functions-describe-execution-output
source_filename: amazon-step-functions-describe-execution-output-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-step-functions/refs/heads/main/json-schema/amazon-step-functions-describe-execution-output-schema.json\",\n  \"title\": \"DescribeExecutionOutput\",\n  \"description\": \"DescribeExecutionOutput schema from Amazon Step Functions API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"executionArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Arn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) that identifies the execution.\"\n        }\n      ]\n    },\n    \"stateMachineArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Arn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the executed stated machine.\"\n        }\n      ]\n    },\n    \"name\": {\n      \"allOf\": [\n        {\n          \"\
  $ref\": \"#/components/schemas/Name\"\n        },\n        {\n          \"description\": \"<p>The name of the execution.</p> <p>A name must <i>not</i> contain:</p> <ul> <li> <p>white space</p> </li> <li> <p>brackets <code>&lt; &gt; { } [ ]</code> </p> </li> <li> <p>wildcard characters <code>? *</code> </p> </li> <li> <p>special characters <code>\\\" # % \\\\ ^ | ~ ` $ &amp; , ; : /</code> </p> </li> <li> <p>control characters (<code>U+0000-001F</code>, <code>U+007F-009F</code>)</p> </li> </ul> <p>To enable logging with CloudWatch Logs, the name should only contain 0-9, A-Z, a-z, - and _.</p>\"\n        }\n      ]\n    },\n    \"status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ExecutionStatus\"\n        },\n        {\n          \"description\": \"The current status of the execution.\"\n        }\n      ]\n    },\n    \"startDate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n     \
  \     \"description\": \"The date the execution is started.\"\n        }\n      ]\n    },\n    \"stopDate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"If the execution ended, the date the execution stopped.\"\n        }\n      ]\n    },\n    \"input\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SensitiveData\"\n        },\n        {\n          \"description\": \"The string that contains the JSON input data of the execution. Length constraints apply to the payload size, and are expressed as bytes in UTF-8 encoding.\"\n        }\n      ]\n    },\n    \"inputDetails\": {\n      \"$ref\": \"#/components/schemas/CloudWatchEventsExecutionDataDetails\"\n    },\n    \"output\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SensitiveData\"\n        },\n        {\n          \"description\": \"<p>The JSON output data of the execution.\
  \ Length constraints apply to the payload size, and are expressed as bytes in UTF-8 encoding.</p> <note> <p>This field is set only if the execution succeeds. If the execution fails, this field is null.</p> </note>\"\n        }\n      ]\n    },\n    \"outputDetails\": {\n      \"$ref\": \"#/components/schemas/CloudWatchEventsExecutionDataDetails\"\n    },\n    \"traceHeader\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TraceHeader\"\n        },\n        {\n          \"description\": \"The X-Ray trace header that was passed to the execution.\"\n        }\n      ]\n    },\n    \"mapRunArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LongArn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) that identifies a Map Run, which dispatched this execution.\"\n        }\n      ]\n    },\n    \"error\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SensitiveError\"\
  \n        },\n        {\n          \"description\": \"The error string if the state machine execution failed.\"\n        }\n      ]\n    },\n    \"cause\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SensitiveCause\"\n        },\n        {\n          \"description\": \"The cause string if the state machine execution failed.\"\n        }\n      ]\n    },\n    \"stateMachineVersionArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Arn\"\n        },\n        {\n          \"description\": \"<p>The Amazon Resource Name (ARN) of the state machine version associated with the execution. The version ARN is a combination of state machine ARN and the version number separated by a colon (:). For example, <code>stateMachineARN:1</code>.</p> <p>If you start an execution from a <code>StartExecution</code> request without specifying a state machine version or alias ARN, Step Functions returns a null value.</p>\"\n        }\n      ]\n  \
  \  },\n    \"stateMachineAliasArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Arn\"\n        },\n        {\n          \"description\": \"<p>The Amazon Resource Name (ARN) of the state machine alias associated with the execution. The alias ARN is a combination of state machine ARN and the alias name separated by a colon (:). For example, <code>stateMachineARN:PROD</code>.</p> <p>If you start an execution from a <code>StartExecution</code> request with a state machine version ARN, this field will be null.</p>\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"executionArn\",\n    \"stateMachineArn\",\n    \"status\",\n    \"startDate\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-step-functions/refs/heads/main/json-schema/amazon-step-functions-describe-execution-output-schema.json
tags:
- AWS
- Orchestration
- Serverless
- State Machine
- Workflow
title: DescribeExecutionOutput
---
