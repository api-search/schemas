---
description: Provides the details of the <code>WorkflowExecutionTerminated</code> event.
layout: schema
name: WorkflowExecutionTerminatedEventAttributes
properties_list:
- description: ''
  name: reason
  type: object
- description: ''
  name: details
  type: object
- description: ''
  name: childPolicy
  type: object
- description: ''
  name: cause
  type: object
provider_name: Amazon Simple Workflow Service
provider_slug: amazon-swf
schema_file: json-schema/amazon-swf-workflowexecutionterminatedeventattributes-schema.json
slug: amazon-swf-workflowexecutionterminatedeventattributes
source_filename: amazon-swf-workflowexecutionterminatedeventattributes-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"required\": [\n    \"childPolicy\"\n  ],\n  \"properties\": {\n    \"reason\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TerminateReason\"\n        },\n        {\n          \"description\": \"The reason provided for the termination.\"\n        }\n      ]\n    },\n    \"details\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Data\"\n        },\n        {\n          \"description\": \"The details provided for the termination.\"\n        }\n      ]\n    },\n    \"childPolicy\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ChildPolicy\"\n        },\n        {\n          \"description\": \"<p>The policy used for the child workflow executions of this workflow execution.</p> <p>The supported child policies are:</p> <ul> <li> <p> <code>TERMINATE</code> \\u2013 The child executions are terminated.</p> </li> <li> <p> <code>REQUEST_CANCEL</code> \\u2013 A\
  \ request to cancel is attempted for each child execution by recording a <code>WorkflowExecutionCancelRequested</code> event in its history. It is up to the decider to take appropriate actions when it receives an execution history with this event.</p> </li> <li> <p> <code>ABANDON</code> \\u2013 No action is taken. The child executions continue to run.</p> </li> </ul>\"\n        }\n      ]\n    },\n    \"cause\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WorkflowExecutionTerminatedCause\"\n        },\n        {\n          \"description\": \"If set, indicates that the workflow execution was automatically terminated, and specifies the cause. This happens if the parent workflow execution times out or is terminated and the child policy is set to terminate child executions.\"\n        }\n      ]\n    }\n  },\n  \"description\": \"Provides the details of the <code>WorkflowExecutionTerminated</code> event.\",\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\"\
  ,\n  \"title\": \"WorkflowExecutionTerminatedEventAttributes\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-swf/refs/heads/main/json-schema/amazon-swf-workflowexecutionterminatedeventattributes-schema.json
tags:
- Automation
- AWS
- Task Coordination
- Workflow
title: WorkflowExecutionTerminatedEventAttributes
---
