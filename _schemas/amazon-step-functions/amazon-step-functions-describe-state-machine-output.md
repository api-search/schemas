---
description: DescribeStateMachineOutput schema from Amazon Step Functions API
layout: schema
name: DescribeStateMachineOutput
properties_list:
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
  name: definition
  type: object
- description: ''
  name: roleArn
  type: object
- description: ''
  name: type
  type: object
- description: ''
  name: creationDate
  type: object
- description: ''
  name: loggingConfiguration
  type: object
- description: ''
  name: tracingConfiguration
  type: object
- description: ''
  name: label
  type: object
- description: ''
  name: revisionId
  type: object
- description: ''
  name: description
  type: object
provider_name: Amazon Step Functions
provider_slug: amazon-step-functions
schema_file: json-schema/amazon-step-functions-describe-state-machine-output-schema.json
slug: amazon-step-functions-describe-state-machine-output
source_filename: amazon-step-functions-describe-state-machine-output-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-step-functions/refs/heads/main/json-schema/amazon-step-functions-describe-state-machine-output-schema.json\",\n  \"title\": \"DescribeStateMachineOutput\",\n  \"description\": \"DescribeStateMachineOutput schema from Amazon Step Functions API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"stateMachineArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Arn\"\n        },\n        {\n          \"description\": \"<p>The Amazon Resource Name (ARN) that identifies the state machine.</p> <p>If you specified a state machine version ARN in your request, the API returns the version ARN. The version ARN is a combination of state machine ARN and the version number separated by a colon (:). For example, <code>stateMachineARN:1</code>.</p>\"\n        }\n      ]\n    },\n    \"name\": {\n      \"allOf\": [\n    \
  \    {\n          \"$ref\": \"#/components/schemas/Name\"\n        },\n        {\n          \"description\": \"<p>The name of the state machine.</p> <p>A name must <i>not</i> contain:</p> <ul> <li> <p>white space</p> </li> <li> <p>brackets <code>&lt; &gt; { } [ ]</code> </p> </li> <li> <p>wildcard characters <code>? *</code> </p> </li> <li> <p>special characters <code>\\\" # % \\\\ ^ | ~ ` $ &amp; , ; : /</code> </p> </li> <li> <p>control characters (<code>U+0000-001F</code>, <code>U+007F-009F</code>)</p> </li> </ul> <p>To enable logging with CloudWatch Logs, the name should only contain 0-9, A-Z, a-z, - and _.</p>\"\n        }\n      ]\n    },\n    \"status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StateMachineStatus\"\n        },\n        {\n          \"description\": \"The current status of the state machine.\"\n        }\n      ]\n    },\n    \"definition\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Definition\"\
  \n        },\n        {\n          \"description\": \"The Amazon States Language definition of the state machine. See <a href=\\\"https://docs.aws.amazon.com/step-functions/latest/dg/concepts-amazon-states-language.html\\\">Amazon States Language</a>.\"\n        }\n      ]\n    },\n    \"roleArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Arn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the IAM role used when creating this state machine. (The IAM role maintains security by granting Step Functions access to Amazon Web Services resources.)\"\n        }\n      ]\n    },\n    \"type\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StateMachineType\"\n        },\n        {\n          \"description\": \"The <code>type</code> of the state machine (<code>STANDARD</code> or <code>EXPRESS</code>).\"\n        }\n      ]\n    },\n    \"creationDate\": {\n      \"allOf\": [\n        {\n  \
  \        \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"<p>The date the state machine is created.</p> <p>For a state machine version, <code>creationDate</code> is the date the version was created.</p>\"\n        }\n      ]\n    },\n    \"loggingConfiguration\": {\n      \"$ref\": \"#/components/schemas/LoggingConfiguration\"\n    },\n    \"tracingConfiguration\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TracingConfiguration\"\n        },\n        {\n          \"description\": \"Selects whether X-Ray tracing is enabled.\"\n        }\n      ]\n    },\n    \"label\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MapRunLabel\"\n        },\n        {\n          \"description\": \"A user-defined or an auto-generated string that identifies a <code>Map</code> state. This parameter is present only if the <code>stateMachineArn</code> specified in input is a qualified state machine\
  \ ARN.\"\n        }\n      ]\n    },\n    \"revisionId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RevisionId\"\n        },\n        {\n          \"description\": \"<p>The revision identifier for the state machine.</p> <p>Use the <code>revisionId</code> parameter to compare between versions of a state machine configuration used for executions without performing a diff of the properties, such as <code>definition</code> and <code>roleArn</code>.</p>\"\n        }\n      ]\n    },\n    \"description\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/VersionDescription\"\n        },\n        {\n          \"description\": \"The description of the state machine version.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"stateMachineArn\",\n    \"name\",\n    \"definition\",\n    \"roleArn\",\n    \"type\",\n    \"creationDate\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-step-functions/refs/heads/main/json-schema/amazon-step-functions-describe-state-machine-output-schema.json
tags:
- Orchestration
- Serverless
- State Machine
- Workflow
title: DescribeStateMachineOutput
---
