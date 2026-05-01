---
description: Provides the details of the <code>WorkflowExecutionSignaled</code> event.
layout: schema
name: WorkflowExecutionSignaledEventAttributes
properties_list:
- description: ''
  name: signalName
  type: object
- description: ''
  name: input
  type: object
- description: ''
  name: externalWorkflowExecution
  type: object
- description: ''
  name: externalInitiatedEventId
  type: object
provider_name: Amazon Simple Workflow Service
provider_slug: amazon-swf
schema_file: json-schema/amazon-swf-workflowexecutionsignaledeventattributes-schema.json
slug: amazon-swf-workflowexecutionsignaledeventattributes
source_filename: amazon-swf-workflowexecutionsignaledeventattributes-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"required\": [\n    \"signalName\"\n  ],\n  \"properties\": {\n    \"signalName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SignalName\"\n        },\n        {\n          \"description\": \"The name of the signal received. The decider can use the signal name and inputs to determine how to the process the signal.\"\n        }\n      ]\n    },\n    \"input\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Data\"\n        },\n        {\n          \"description\": \"The inputs provided with the signal. The decider can use the signal name and inputs to determine how to process the signal.\"\n        }\n      ]\n    },\n    \"externalWorkflowExecution\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WorkflowExecution\"\n        },\n        {\n          \"description\": \"The workflow execution that sent the signal. This is set only of the signal was sent\
  \ by another workflow execution.\"\n        }\n      ]\n    },\n    \"externalInitiatedEventId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EventId\"\n        },\n        {\n          \"description\": \"The ID of the <code>SignalExternalWorkflowExecutionInitiated</code> event corresponding to the <code>SignalExternalWorkflow</code> decision to signal this workflow execution.The source event with this ID can be found in the history of the source workflow execution. This information can be useful for diagnosing problems by tracing back the chain of events leading up to this event. This field is set only if the signal was initiated by another workflow execution.\"\n        }\n      ]\n    }\n  },\n  \"description\": \"Provides the details of the <code>WorkflowExecutionSignaled</code> event.\",\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"WorkflowExecutionSignaledEventAttributes\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-swf/refs/heads/main/json-schema/amazon-swf-workflowexecutionsignaledeventattributes-schema.json
tags:
- Automation
- Task Coordination
- Workflow
title: WorkflowExecutionSignaledEventAttributes
---
