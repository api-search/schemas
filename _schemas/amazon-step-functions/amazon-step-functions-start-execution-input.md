---
description: StartExecutionInput schema from Amazon Step Functions API
layout: schema
name: StartExecutionInput
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
schema_file: json-schema/amazon-step-functions-start-execution-input-schema.json
slug: amazon-step-functions-start-execution-input
source_filename: amazon-step-functions-start-execution-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-step-functions/refs/heads/main/json-schema/amazon-step-functions-start-execution-input-schema.json\",\n  \"title\": \"StartExecutionInput\",\n  \"description\": \"StartExecutionInput schema from Amazon Step Functions API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"stateMachineArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Arn\"\n        },\n        {\n          \"description\": \"<p>The Amazon Resource Name (ARN) of the state machine to execute.</p> <p>The <code>stateMachineArn</code> parameter accepts one of the following inputs:</p> <ul> <li> <p> <b>An unqualified state machine ARN</b> \\u2013 Refers to a state machine ARN that isn't qualified with a version or alias ARN. The following is an example of an unqualified state machine ARN.</p> <p> <code>arn:&lt;partition&gt;:states:&lt;region&gt;:&lt;account-id&gt;:stateMachine:&lt;myStateMachine&gt;</code>\
  \ </p> <p>Step Functions doesn't associate state machine executions that you start with an unqualified ARN with a version. This is true even if that version uses the same revision that the execution used.</p> </li> <li> <p> <b>A state machine version ARN</b> \\u2013 Refers to a version ARN, which is a combination of state machine ARN and the version number separated by a colon (:). The following is an example of the ARN for version 10. </p> <p> <code>arn:&lt;partition&gt;:states:&lt;region&gt;:&lt;account-id&gt;:stateMachine:&lt;myStateMachine&gt;:10</code> </p> <p>Step Functions doesn't associate executions that you start with a version ARN with any aliases that point to that version.</p> </li> <li> <p> <b>A state machine alias ARN</b> \\u2013 Refers to an alias ARN, which is a combination of state machine ARN and the alias name separated by a colon (:). The following is an example of the ARN for an alias named <code>PROD</code>.</p> <p> <code>arn:&lt;partition&gt;:states:&lt;region&gt;:&lt;account-id&gt;:stateMachine:&lt;myStateMachine:PROD&gt;</code>\
  \ </p> <p>Step Functions associates executions that you start with an alias ARN with that alias and the state machine version used for that execution.</p> </li> </ul>\"\n        }\n      ]\n    },\n    \"name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Name\"\n        },\n        {\n          \"description\": \"<p>Optional name of the execution. This name must be unique for your Amazon Web Services account, Region, and state machine for 90 days. For more information, see <a href=\\\"https://docs.aws.amazon.com/step-functions/latest/dg/limits.html#service-limits-state-machine-executions\\\"> Limits Related to State Machine Executions</a> in the <i>Step Functions Developer Guide</i>.</p> <p>A name must <i>not</i> contain:</p> <ul> <li> <p>white space</p> </li> <li> <p>brackets <code>&lt; &gt; { } [ ]</code> </p> </li> <li> <p>wildcard characters <code>? *</code> </p> </li> <li> <p>special characters <code>\\\" # % \\\\ ^ | ~ ` $ &amp; , ; : /</code> </p>\
  \ </li> <li> <p>control characters (<code>U+0000-001F</code>, <code>U+007F-009F</code>)</p> </li> </ul> <p>To enable logging with CloudWatch Logs, the name should only contain 0-9, A-Z, a-z, - and _.</p>\"\n        }\n      ]\n    },\n    \"input\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SensitiveData\"\n        },\n        {\n          \"description\": \"<p>The string that contains the JSON input data for the execution, for example:</p> <p> <code>\\\"input\\\": \\\"{\\\\\\\"first_name\\\\\\\" : \\\\\\\"test\\\\\\\"}\\\"</code> </p> <note> <p>If you don't include any JSON input data, you still must include the two braces, for example: <code>\\\"input\\\": \\\"{}\\\"</code> </p> </note> <p>Length constraints apply to the payload size, and are expressed as bytes in UTF-8 encoding.</p>\"\n        }\n      ]\n    },\n    \"traceHeader\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TraceHeader\"\n        },\n        {\n\
  \          \"description\": \"Passes the X-Ray trace header. The trace header can also be passed in the request payload.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"stateMachineArn\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-step-functions/refs/heads/main/json-schema/amazon-step-functions-start-execution-input-schema.json
tags:
- Orchestration
- Serverless
- State Machine
- Workflow
title: StartExecutionInput
---
