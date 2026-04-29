---
description: CreateStateMachineInput schema from Amazon Step Functions API
layout: schema
name: CreateStateMachineInput
properties_list:
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
  name: type
  type: object
- description: ''
  name: loggingConfiguration
  type: object
- description: ''
  name: tags
  type: object
- description: ''
  name: tracingConfiguration
  type: object
- description: ''
  name: publish
  type: object
- description: ''
  name: versionDescription
  type: object
provider_name: Amazon Step Functions
provider_slug: amazon-step-functions
schema_file: json-schema/amazon-step-functions-create-state-machine-input-schema.json
slug: amazon-step-functions-create-state-machine-input
source_filename: amazon-step-functions-create-state-machine-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-step-functions/refs/heads/main/json-schema/amazon-step-functions-create-state-machine-input-schema.json\",\n  \"title\": \"CreateStateMachineInput\",\n  \"description\": \"CreateStateMachineInput schema from Amazon Step Functions API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Name\"\n        },\n        {\n          \"description\": \"<p>The name of the state machine. </p> <p>A name must <i>not</i> contain:</p> <ul> <li> <p>white space</p> </li> <li> <p>brackets <code>&lt; &gt; { } [ ]</code> </p> </li> <li> <p>wildcard characters <code>? *</code> </p> </li> <li> <p>special characters <code>\\\" # % \\\\ ^ | ~ ` $ &amp; , ; : /</code> </p> </li> <li> <p>control characters (<code>U+0000-001F</code>, <code>U+007F-009F</code>)</p> </li> </ul> <p>To\
  \ enable logging with CloudWatch Logs, the name should only contain 0-9, A-Z, a-z, - and _.</p>\"\n        }\n      ]\n    },\n    \"definition\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Definition\"\n        },\n        {\n          \"description\": \"The Amazon States Language definition of the state machine. See <a href=\\\"https://docs.aws.amazon.com/step-functions/latest/dg/concepts-amazon-states-language.html\\\">Amazon States Language</a>.\"\n        }\n      ]\n    },\n    \"roleArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Arn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the IAM role to use for this state machine.\"\n        }\n      ]\n    },\n    \"type\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StateMachineType\"\n        },\n        {\n          \"description\": \"Determines whether a Standard or Express state machine is\
  \ created. The default is <code>STANDARD</code>. You cannot update the <code>type</code> of a state machine once it has been created.\"\n        }\n      ]\n    },\n    \"loggingConfiguration\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LoggingConfiguration\"\n        },\n        {\n          \"description\": \"<p>Defines what execution history events are logged and where they are logged.</p> <note> <p>By default, the <code>level</code> is set to <code>OFF</code>. For more information see <a href=\\\"https://docs.aws.amazon.com/step-functions/latest/dg/cloudwatch-log-level.html\\\">Log Levels</a> in the Step Functions User Guide.</p> </note>\"\n        }\n      ]\n    },\n    \"tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TagList\"\n        },\n        {\n          \"description\": \"<p>Tags to be added when creating a state machine.</p> <p>An array of key-value pairs. For more information, see <a href=\\\"https://docs.aws.amazon.com/awsaccountbilling/latest/aboutv2/cost-alloc-tags.html\\\
  \">Using Cost Allocation Tags</a> in the <i>Amazon Web Services Billing and Cost Management User Guide</i>, and <a href=\\\"https://docs.aws.amazon.com/IAM/latest/UserGuide/access_iam-tags.html\\\">Controlling Access Using IAM Tags</a>.</p> <p>Tags may only contain Unicode letters, digits, white space, or these symbols: <code>_ . : / = + - @</code>.</p>\"\n        }\n      ]\n    },\n    \"tracingConfiguration\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TracingConfiguration\"\n        },\n        {\n          \"description\": \"Selects whether X-Ray tracing is enabled.\"\n        }\n      ]\n    },\n    \"publish\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Publish\"\n        },\n        {\n          \"description\": \"Set to <code>true</code> to publish the first version of the state machine during creation. The default is <code>false</code>.\"\n        }\n      ]\n    },\n    \"versionDescription\": {\n      \"allOf\"\
  : [\n        {\n          \"$ref\": \"#/components/schemas/VersionDescription\"\n        },\n        {\n          \"description\": \"Sets description about the state machine version. You can only set the description if the <code>publish</code> parameter is set to <code>true</code>. Otherwise, if you set <code>versionDescription</code>, but <code>publish</code> to <code>false</code>, this API action throws <code>ValidationException</code>.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"name\",\n    \"definition\",\n    \"roleArn\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-step-functions/refs/heads/main/json-schema/amazon-step-functions-create-state-machine-input-schema.json
tags:
- AWS
- Orchestration
- Serverless
- State Machine
- Workflow
title: CreateStateMachineInput
---
