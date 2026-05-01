---
description: Provides the details of the <code>ChildWorkflowExecutionTimedOut</code> event.
layout: schema
name: ChildWorkflowExecutionTimedOutEventAttributes
properties_list:
- description: ''
  name: workflowExecution
  type: object
- description: ''
  name: workflowType
  type: object
- description: ''
  name: timeoutType
  type: object
- description: ''
  name: initiatedEventId
  type: object
- description: ''
  name: startedEventId
  type: object
provider_name: Amazon Simple Workflow Service
provider_slug: amazon-swf
schema_file: json-schema/amazon-swf-childworkflowexecutiontimedouteventattributes-schema.json
slug: amazon-swf-childworkflowexecutiontimedouteventattributes
source_filename: amazon-swf-childworkflowexecutiontimedouteventattributes-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"required\": [\n    \"workflowExecution\",\n    \"workflowType\",\n    \"timeoutType\",\n    \"initiatedEventId\",\n    \"startedEventId\"\n  ],\n  \"properties\": {\n    \"workflowExecution\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WorkflowExecution\"\n        },\n        {\n          \"description\": \"The child workflow execution that timed out.\"\n        }\n      ]\n    },\n    \"workflowType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WorkflowType\"\n        },\n        {\n          \"description\": \"The type of the child workflow execution.\"\n        }\n      ]\n    },\n    \"timeoutType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WorkflowExecutionTimeoutType\"\n        },\n        {\n          \"description\": \"The type of the timeout that caused the child workflow execution to time out.\"\n        }\n      ]\n    },\n    \"\
  initiatedEventId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EventId\"\n        },\n        {\n          \"description\": \"The ID of the <code>StartChildWorkflowExecutionInitiated</code> event corresponding to the <code>StartChildWorkflowExecution</code> <a>Decision</a> to start this child workflow execution. This information can be useful for diagnosing problems by tracing back the chain of events leading up to this event.\"\n        }\n      ]\n    },\n    \"startedEventId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EventId\"\n        },\n        {\n          \"description\": \"The ID of the <code>ChildWorkflowExecutionStarted</code> event recorded when this child workflow execution was started. This information can be useful for diagnosing problems by tracing back the chain of events leading up to this event.\"\n        }\n      ]\n    }\n  },\n  \"description\": \"Provides the details of the <code>ChildWorkflowExecutionTimedOut</code>\
  \ event.\",\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"ChildWorkflowExecutionTimedOutEventAttributes\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-swf/refs/heads/main/json-schema/amazon-swf-childworkflowexecutiontimedouteventattributes-schema.json
tags:
- Automation
- Task Coordination
- Workflow
title: ChildWorkflowExecutionTimedOutEventAttributes
---
