---
description: Provides the details of the <code>ExternalWorkflowExecutionSignaled</code> event.
layout: schema
name: ExternalWorkflowExecutionSignaledEventAttributes
properties_list:
- description: ''
  name: workflowExecution
  type: object
- description: ''
  name: initiatedEventId
  type: object
provider_name: Amazon Simple Workflow Service
provider_slug: amazon-swf
schema_file: json-schema/amazon-swf-externalworkflowexecutionsignaledeventattributes-schema.json
slug: amazon-swf-externalworkflowexecutionsignaledeventattributes
source_filename: amazon-swf-externalworkflowexecutionsignaledeventattributes-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"required\": [\n    \"workflowExecution\",\n    \"initiatedEventId\"\n  ],\n  \"properties\": {\n    \"workflowExecution\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WorkflowExecution\"\n        },\n        {\n          \"description\": \"The external workflow execution that the signal was delivered to.\"\n        }\n      ]\n    },\n    \"initiatedEventId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EventId\"\n        },\n        {\n          \"description\": \"The ID of the <code>SignalExternalWorkflowExecutionInitiated</code> event corresponding to the <code>SignalExternalWorkflowExecution</code> decision to request this signal. This information can be useful for diagnosing problems by tracing back the chain of events leading up to this event.\"\n        }\n      ]\n    }\n  },\n  \"description\": \"Provides the details of the <code>ExternalWorkflowExecutionSignaled</code>\
  \ event.\",\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"ExternalWorkflowExecutionSignaledEventAttributes\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-swf/refs/heads/main/json-schema/amazon-swf-externalworkflowexecutionsignaledeventattributes-schema.json
tags:
- Automation
- Task Coordination
- Workflow
title: ExternalWorkflowExecutionSignaledEventAttributes
---
