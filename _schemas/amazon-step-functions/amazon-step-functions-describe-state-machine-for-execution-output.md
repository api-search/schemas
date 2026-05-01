---
description: DescribeStateMachineForExecutionOutput schema from Amazon Step Functions API
layout: schema
name: DescribeStateMachineForExecutionOutput
properties_list:
- description: ''
  name: stateMachineArn
  type: object
- description: ''
  name: name
  type: object
- description: ''
  name: definition
  type: object
- description: ''
  name: roleArn
  type: object
- description: ''
  name: updateDate
  type: object
- description: ''
  name: loggingConfiguration
  type: object
- description: ''
  name: tracingConfiguration
  type: object
- description: ''
  name: mapRunArn
  type: object
- description: ''
  name: label
  type: object
- description: ''
  name: revisionId
  type: object
provider_name: Amazon Step Functions
provider_slug: amazon-step-functions
schema_file: json-schema/amazon-step-functions-describe-state-machine-for-execution-output-schema.json
slug: amazon-step-functions-describe-state-machine-for-execution-output
source_filename: amazon-step-functions-describe-state-machine-for-execution-output-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-step-functions/refs/heads/main/json-schema/amazon-step-functions-describe-state-machine-for-execution-output-schema.json\",\n  \"title\": \"DescribeStateMachineForExecutionOutput\",\n  \"description\": \"DescribeStateMachineForExecutionOutput schema from Amazon Step Functions API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"stateMachineArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Arn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the state machine associated with the execution.\"\n        }\n      ]\n    },\n    \"name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Name\"\n        },\n        {\n          \"description\": \"The name of the state machine associated with the execution.\"\n        }\n      ]\n    },\n\
  \    \"definition\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Definition\"\n        },\n        {\n          \"description\": \"The Amazon States Language definition of the state machine. See <a href=\\\"https://docs.aws.amazon.com/step-functions/latest/dg/concepts-amazon-states-language.html\\\">Amazon States Language</a>.\"\n        }\n      ]\n    },\n    \"roleArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Arn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the IAM role of the State Machine for the execution. \"\n        }\n      ]\n    },\n    \"updateDate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The date and time the state machine associated with an execution was updated. For a newly created state machine, this is the creation date.\"\n        }\n      ]\n    },\n \
  \   \"loggingConfiguration\": {\n      \"$ref\": \"#/components/schemas/LoggingConfiguration\"\n    },\n    \"tracingConfiguration\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TracingConfiguration\"\n        },\n        {\n          \"description\": \"Selects whether X-Ray tracing is enabled.\"\n        }\n      ]\n    },\n    \"mapRunArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LongArn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the Map Run that started the child workflow execution. This field is returned only if the <code>executionArn</code> is a child workflow execution that was started by a Distributed Map state.\"\n        }\n      ]\n    },\n    \"label\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MapRunLabel\"\n        },\n        {\n          \"description\": \"A user-defined or an auto-generated string that identifies a <code>Map</code>\
  \ state. This \\ufb01eld is returned only if the <code>executionArn</code> is a child workflow execution that was started by a Distributed Map state.\"\n        }\n      ]\n    },\n    \"revisionId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RevisionId\"\n        },\n        {\n          \"description\": \"<p>The revision identifier for the state machine. The first revision ID when you create the state machine is null.</p> <p>Use the state machine <code>revisionId</code> parameter to compare the revision of a state machine with the configuration of the state machine used for executions without performing a diff of the properties, such as <code>definition</code> and <code>roleArn</code>.</p>\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"stateMachineArn\",\n    \"name\",\n    \"definition\",\n    \"roleArn\",\n    \"updateDate\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-step-functions/refs/heads/main/json-schema/amazon-step-functions-describe-state-machine-for-execution-output-schema.json
tags:
- Orchestration
- Serverless
- State Machine
- Workflow
title: DescribeStateMachineForExecutionOutput
---
