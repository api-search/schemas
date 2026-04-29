---
description: ''
layout: schema
name: TerminateWorkflowExecutionInput
properties_list:
- description: ''
  name: domain
  type: object
- description: ''
  name: workflowId
  type: object
- description: ''
  name: runId
  type: object
- description: ''
  name: reason
  type: object
- description: ''
  name: details
  type: object
- description: ''
  name: childPolicy
  type: object
provider_name: Amazon Simple Workflow Service
provider_slug: amazon-swf
schema_file: json-schema/amazon-swf-terminateworkflowexecutioninput-schema.json
slug: amazon-swf-terminateworkflowexecutioninput
source_filename: amazon-swf-terminateworkflowexecutioninput-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"required\": [\n    \"domain\",\n    \"workflowId\"\n  ],\n  \"title\": \"TerminateWorkflowExecutionInput\",\n  \"properties\": {\n    \"domain\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DomainName\"\n        },\n        {\n          \"description\": \"The domain of the workflow execution to terminate.\"\n        }\n      ]\n    },\n    \"workflowId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WorkflowId\"\n        },\n        {\n          \"description\": \"The workflowId of the workflow execution to terminate.\"\n        }\n      ]\n    },\n    \"runId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WorkflowRunIdOptional\"\n        },\n        {\n          \"description\": \"The runId of the workflow execution to terminate.\"\n        }\n      ]\n    },\n    \"reason\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TerminateReason\"\
  \n        },\n        {\n          \"description\": \" A descriptive reason for terminating the workflow execution.\"\n        }\n      ]\n    },\n    \"details\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Data\"\n        },\n        {\n          \"description\": \" Details for terminating the workflow execution.\"\n        }\n      ]\n    },\n    \"childPolicy\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ChildPolicy\"\n        },\n        {\n          \"description\": \"<p>If set, specifies the policy to use for the child workflow executions of the workflow execution being terminated. This policy overrides the child policy specified for the workflow execution at registration time or when starting the execution.</p> <p>The supported child policies are:</p> <ul> <li> <p> <code>TERMINATE</code> \\u2013 The child executions are terminated.</p> </li> <li> <p> <code>REQUEST_CANCEL</code> \\u2013 A request to cancel is attempted\
  \ for each child execution by recording a <code>WorkflowExecutionCancelRequested</code> event in its history. It is up to the decider to take appropriate actions when it receives an execution history with this event.</p> </li> <li> <p> <code>ABANDON</code> \\u2013 No action is taken. The child executions continue to run.</p> </li> </ul> <note> <p>A child policy for this workflow execution must be specified either as a default for the workflow type or through this parameter. If neither this parameter is set nor a default child policy was specified at registration time then a fault is returned.</p> </note>\"\n        }\n      ]\n    }\n  },\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-swf/refs/heads/main/json-schema/amazon-swf-terminateworkflowexecutioninput-schema.json
tags:
- Automation
- AWS
- Task Coordination
- Workflow
title: TerminateWorkflowExecutionInput
---
