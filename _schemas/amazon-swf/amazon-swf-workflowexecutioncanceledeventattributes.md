---
description: Provides the details of the <code>WorkflowExecutionCanceled</code> event.
layout: schema
name: WorkflowExecutionCanceledEventAttributes
properties_list:
- description: ''
  name: details
  type: object
- description: ''
  name: decisionTaskCompletedEventId
  type: object
provider_name: Amazon Simple Workflow Service
provider_slug: amazon-swf
schema_file: json-schema/amazon-swf-workflowexecutioncanceledeventattributes-schema.json
slug: amazon-swf-workflowexecutioncanceledeventattributes
source_filename: amazon-swf-workflowexecutioncanceledeventattributes-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"required\": [\n    \"decisionTaskCompletedEventId\"\n  ],\n  \"properties\": {\n    \"details\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Data\"\n        },\n        {\n          \"description\": \"The details of the cancellation.\"\n        }\n      ]\n    },\n    \"decisionTaskCompletedEventId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EventId\"\n        },\n        {\n          \"description\": \"The ID of the <code>DecisionTaskCompleted</code> event corresponding to the decision task that resulted in the <code>CancelWorkflowExecution</code> decision for this cancellation request. This information can be useful for diagnosing problems by tracing back the chain of events leading up to this event.\"\n        }\n      ]\n    }\n  },\n  \"description\": \"Provides the details of the <code>WorkflowExecutionCanceled</code> event.\",\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\"\
  ,\n  \"title\": \"WorkflowExecutionCanceledEventAttributes\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-swf/refs/heads/main/json-schema/amazon-swf-workflowexecutioncanceledeventattributes-schema.json
tags:
- Automation
- AWS
- Task Coordination
- Workflow
title: WorkflowExecutionCanceledEventAttributes
---
