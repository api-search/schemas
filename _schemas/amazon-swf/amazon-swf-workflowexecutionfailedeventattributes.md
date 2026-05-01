---
description: Provides the details of the <code>WorkflowExecutionFailed</code> event.
layout: schema
name: WorkflowExecutionFailedEventAttributes
properties_list:
- description: ''
  name: reason
  type: object
- description: ''
  name: details
  type: object
- description: ''
  name: decisionTaskCompletedEventId
  type: object
provider_name: Amazon Simple Workflow Service
provider_slug: amazon-swf
schema_file: json-schema/amazon-swf-workflowexecutionfailedeventattributes-schema.json
slug: amazon-swf-workflowexecutionfailedeventattributes
source_filename: amazon-swf-workflowexecutionfailedeventattributes-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"required\": [\n    \"decisionTaskCompletedEventId\"\n  ],\n  \"properties\": {\n    \"reason\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FailureReason\"\n        },\n        {\n          \"description\": \"The descriptive reason provided for the failure.\"\n        }\n      ]\n    },\n    \"details\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Data\"\n        },\n        {\n          \"description\": \"The details of the failure.\"\n        }\n      ]\n    },\n    \"decisionTaskCompletedEventId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EventId\"\n        },\n        {\n          \"description\": \"The ID of the <code>DecisionTaskCompleted</code> event corresponding to the decision task that resulted in the <code>FailWorkflowExecution</code> decision to fail this execution. This information can be useful for diagnosing problems by tracing\
  \ back the chain of events leading up to this event.\"\n        }\n      ]\n    }\n  },\n  \"description\": \"Provides the details of the <code>WorkflowExecutionFailed</code> event.\",\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"WorkflowExecutionFailedEventAttributes\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-swf/refs/heads/main/json-schema/amazon-swf-workflowexecutionfailedeventattributes-schema.json
tags:
- Automation
- Task Coordination
- Workflow
title: WorkflowExecutionFailedEventAttributes
---
