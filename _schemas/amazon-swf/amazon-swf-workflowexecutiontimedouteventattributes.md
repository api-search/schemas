---
description: Provides the details of the <code>WorkflowExecutionTimedOut</code> event.
layout: schema
name: WorkflowExecutionTimedOutEventAttributes
properties_list:
- description: ''
  name: timeoutType
  type: object
- description: ''
  name: childPolicy
  type: object
provider_name: Amazon Simple Workflow Service
provider_slug: amazon-swf
schema_file: json-schema/amazon-swf-workflowexecutiontimedouteventattributes-schema.json
slug: amazon-swf-workflowexecutiontimedouteventattributes
source_filename: amazon-swf-workflowexecutiontimedouteventattributes-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"required\": [\n    \"timeoutType\",\n    \"childPolicy\"\n  ],\n  \"properties\": {\n    \"timeoutType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WorkflowExecutionTimeoutType\"\n        },\n        {\n          \"description\": \"The type of timeout that caused this event.\"\n        }\n      ]\n    },\n    \"childPolicy\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ChildPolicy\"\n        },\n        {\n          \"description\": \"<p>The policy used for the child workflow executions of this workflow execution.</p> <p>The supported child policies are:</p> <ul> <li> <p> <code>TERMINATE</code> \\u2013 The child executions are terminated.</p> </li> <li> <p> <code>REQUEST_CANCEL</code> \\u2013 A request to cancel is attempted for each child execution by recording a <code>WorkflowExecutionCancelRequested</code> event in its history. It is up to the decider to take appropriate actions\
  \ when it receives an execution history with this event.</p> </li> <li> <p> <code>ABANDON</code> \\u2013 No action is taken. The child executions continue to run.</p> </li> </ul>\"\n        }\n      ]\n    }\n  },\n  \"description\": \"Provides the details of the <code>WorkflowExecutionTimedOut</code> event.\",\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"WorkflowExecutionTimedOutEventAttributes\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-swf/refs/heads/main/json-schema/amazon-swf-workflowexecutiontimedouteventattributes-schema.json
tags:
- Automation
- AWS
- Task Coordination
- Workflow
title: WorkflowExecutionTimedOutEventAttributes
---
