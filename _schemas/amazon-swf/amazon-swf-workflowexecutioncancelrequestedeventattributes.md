---
description: Provides the details of the <code>WorkflowExecutionCancelRequested</code> event.
layout: schema
name: WorkflowExecutionCancelRequestedEventAttributes
properties_list:
- description: ''
  name: externalWorkflowExecution
  type: object
- description: ''
  name: externalInitiatedEventId
  type: object
- description: ''
  name: cause
  type: object
provider_name: Amazon Simple Workflow Service
provider_slug: amazon-swf
schema_file: json-schema/amazon-swf-workflowexecutioncancelrequestedeventattributes-schema.json
slug: amazon-swf-workflowexecutioncancelrequestedeventattributes
source_filename: amazon-swf-workflowexecutioncancelrequestedeventattributes-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"externalWorkflowExecution\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WorkflowExecution\"\n        },\n        {\n          \"description\": \"The external workflow execution for which the cancellation was requested.\"\n        }\n      ]\n    },\n    \"externalInitiatedEventId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EventId\"\n        },\n        {\n          \"description\": \"The ID of the <code>RequestCancelExternalWorkflowExecutionInitiated</code> event corresponding to the <code>RequestCancelExternalWorkflowExecution</code> decision to cancel this workflow execution.The source event with this ID can be found in the history of the source workflow execution. This information can be useful for diagnosing problems by tracing back the chain of events leading up to this event.\"\n        }\n      ]\n    },\n    \"cause\": {\n      \"allOf\": [\n\
  \        {\n          \"$ref\": \"#/components/schemas/WorkflowExecutionCancelRequestedCause\"\n        },\n        {\n          \"description\": \"If set, indicates that the request to cancel the workflow execution was automatically generated, and specifies the cause. This happens if the parent workflow execution times out or is terminated, and the child policy is set to cancel child executions.\"\n        }\n      ]\n    }\n  },\n  \"description\": \"Provides the details of the <code>WorkflowExecutionCancelRequested</code> event.\",\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"WorkflowExecutionCancelRequestedEventAttributes\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-swf/refs/heads/main/json-schema/amazon-swf-workflowexecutioncancelrequestedeventattributes-schema.json
tags:
- Automation
- Task Coordination
- Workflow
title: WorkflowExecutionCancelRequestedEventAttributes
---
