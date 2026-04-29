---
description: Provides the details of the <code>RequestCancelExternalWorkflowExecutionInitiated</code> event.
layout: schema
name: RequestCancelExternalWorkflowExecutionInitiatedEventAttributes
properties_list:
- description: ''
  name: workflowId
  type: object
- description: ''
  name: runId
  type: object
- description: ''
  name: decisionTaskCompletedEventId
  type: object
- description: ''
  name: control
  type: object
provider_name: Amazon Simple Workflow Service
provider_slug: amazon-swf
schema_file: json-schema/amazon-swf-requestcancelexternalworkflowexecutioninitiatedeventattributes-schema.json
slug: amazon-swf-requestcancelexternalworkflowexecutioninitiatedeventattributes
source_filename: amazon-swf-requestcancelexternalworkflowexecutioninitiatedeventattributes-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"required\": [\n    \"workflowId\",\n    \"decisionTaskCompletedEventId\"\n  ],\n  \"properties\": {\n    \"workflowId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WorkflowId\"\n        },\n        {\n          \"description\": \"The <code>workflowId</code> of the external workflow execution to be canceled.\"\n        }\n      ]\n    },\n    \"runId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WorkflowRunIdOptional\"\n        },\n        {\n          \"description\": \"The <code>runId</code> of the external workflow execution to be canceled.\"\n        }\n      ]\n    },\n    \"decisionTaskCompletedEventId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EventId\"\n        },\n        {\n          \"description\": \"The ID of the <code>DecisionTaskCompleted</code> event corresponding to the decision task that resulted in the <code>RequestCancelExternalWorkflowExecution</code>\
  \ decision for this cancellation request. This information can be useful for diagnosing problems by tracing back the chain of events leading up to this event.\"\n        }\n      ]\n    },\n    \"control\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Data\"\n        },\n        {\n          \"description\": \"Data attached to the event that can be used by the decider in subsequent workflow tasks.\"\n        }\n      ]\n    }\n  },\n  \"description\": \"Provides the details of the <code>RequestCancelExternalWorkflowExecutionInitiated</code> event.\",\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"RequestCancelExternalWorkflowExecutionInitiatedEventAttributes\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-swf/refs/heads/main/json-schema/amazon-swf-requestcancelexternalworkflowexecutioninitiatedeventattributes-schema.json
tags:
- Automation
- AWS
- Task Coordination
- Workflow
title: RequestCancelExternalWorkflowExecutionInitiatedEventAttributes
---
