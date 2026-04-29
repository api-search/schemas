---
description: StartSyncExecutionOutput schema from Amazon Step Functions API
layout: schema
name: StartSyncExecutionOutput
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
  name: startDate
  type: object
- description: ''
  name: stopDate
  type: object
- description: ''
  name: status
  type: object
- description: ''
  name: error
  type: object
- description: ''
  name: cause
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
  name: billingDetails
  type: object
provider_name: Amazon Step Functions
provider_slug: amazon-step-functions
schema_file: json-schema/amazon-step-functions-start-sync-execution-output-schema.json
slug: amazon-step-functions-start-sync-execution-output
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-step-functions/refs/heads/main/json-schema/amazon-step-functions-start-sync-execution-output-schema.json\",\n  \"title\": \"StartSyncExecutionOutput\",\n  \"description\": \"StartSyncExecutionOutput schema from Amazon Step Functions API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"executionArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Arn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) that identifies the execution.\"\n        }\n      ]\n    },\n    \"stateMachineArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Arn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) that identifies the state machine.\"\n        }\n      ]\n    },\n    \"name\": {\n      \"allOf\": [\n        {\n     \
  \     \"$ref\": \"#/components/schemas/Name\"\n        },\n        {\n          \"description\": \"The name of the execution.\"\n        }\n      ]\n    },\n    \"startDate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The date the execution is started.\"\n        }\n      ]\n    },\n    \"stopDate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"If the execution has already ended, the date the execution stopped.\"\n        }\n      ]\n    },\n    \"status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SyncExecutionStatus\"\n        },\n        {\n          \"description\": \"The current status of the execution.\"\n        }\n      ]\n    },\n    \"error\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SensitiveError\"\n        },\n\
  \        {\n          \"description\": \"The error code of the failure.\"\n        }\n      ]\n    },\n    \"cause\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SensitiveCause\"\n        },\n        {\n          \"description\": \"A more detailed explanation of the cause of the failure.\"\n        }\n      ]\n    },\n    \"input\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SensitiveData\"\n        },\n        {\n          \"description\": \"The string that contains the JSON input data of the execution. Length constraints apply to the payload size, and are expressed as bytes in UTF-8 encoding.\"\n        }\n      ]\n    },\n    \"inputDetails\": {\n      \"$ref\": \"#/components/schemas/CloudWatchEventsExecutionDataDetails\"\n    },\n    \"output\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SensitiveData\"\n        },\n        {\n          \"description\": \"<p>The JSON output data of\
  \ the execution. Length constraints apply to the payload size, and are expressed as bytes in UTF-8 encoding.</p> <note> <p>This field is set only if the execution succeeds. If the execution fails, this field is null.</p> </note>\"\n        }\n      ]\n    },\n    \"outputDetails\": {\n      \"$ref\": \"#/components/schemas/CloudWatchEventsExecutionDataDetails\"\n    },\n    \"traceHeader\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TraceHeader\"\n        },\n        {\n          \"description\": \"The X-Ray trace header that was passed to the execution.\"\n        }\n      ]\n    },\n    \"billingDetails\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BillingDetails\"\n        },\n        {\n          \"description\": \"An object that describes workflow billing details, including billed duration and memory use.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"executionArn\",\n    \"startDate\",\n    \"stopDate\"\
  ,\n    \"status\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-step-functions/refs/heads/main/json-schema/amazon-step-functions-start-sync-execution-output-schema.json
tags:
- AWS
- Orchestration
- Serverless
- State Machine
- Workflow
title: StartSyncExecutionOutput
---
