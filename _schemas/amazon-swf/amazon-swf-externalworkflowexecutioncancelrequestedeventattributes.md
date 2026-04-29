---
description: Provides the details of the <code>ExternalWorkflowExecutionCancelRequested</code> event.
layout: schema
name: ExternalWorkflowExecutionCancelRequestedEventAttributes
properties_list:
- description: ''
  name: workflowExecution
  type: object
- description: ''
  name: initiatedEventId
  type: object
provider_name: Amazon Simple Workflow Service
provider_slug: amazon-swf
schema_file: json-schema/amazon-swf-externalworkflowexecutioncancelrequestedeventattributes-schema.json
slug: amazon-swf-externalworkflowexecutioncancelrequestedeventattributes
source_filename: amazon-swf-externalworkflowexecutioncancelrequestedeventattributes-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"required\": [\n    \"workflowExecution\",\n    \"initiatedEventId\"\n  ],\n  \"properties\": {\n    \"workflowExecution\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WorkflowExecution\"\n        },\n        {\n          \"description\": \"The external workflow execution to which the cancellation request was delivered.\"\n        }\n      ]\n    },\n    \"initiatedEventId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EventId\"\n        },\n        {\n          \"description\": \"The ID of the <code>RequestCancelExternalWorkflowExecutionInitiated</code> event corresponding to the <code>RequestCancelExternalWorkflowExecution</code> decision to cancel this external workflow execution. This information can be useful for diagnosing problems by tracing back the chain of events leading up to this event.\"\n        }\n      ]\n    }\n  },\n  \"description\": \"Provides the details of\
  \ the <code>ExternalWorkflowExecutionCancelRequested</code> event.\",\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"ExternalWorkflowExecutionCancelRequestedEventAttributes\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-swf/refs/heads/main/json-schema/amazon-swf-externalworkflowexecutioncancelrequestedeventattributes-schema.json
tags:
- Automation
- AWS
- Task Coordination
- Workflow
title: ExternalWorkflowExecutionCancelRequestedEventAttributes
---
