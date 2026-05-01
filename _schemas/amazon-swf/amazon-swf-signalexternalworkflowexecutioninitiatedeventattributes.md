---
description: Provides the details of the <code>SignalExternalWorkflowExecutionInitiated</code> event.
layout: schema
name: SignalExternalWorkflowExecutionInitiatedEventAttributes
properties_list:
- description: ''
  name: workflowId
  type: object
- description: ''
  name: runId
  type: object
- description: ''
  name: signalName
  type: object
- description: ''
  name: input
  type: object
- description: ''
  name: decisionTaskCompletedEventId
  type: object
- description: ''
  name: control
  type: object
provider_name: Amazon Simple Workflow Service
provider_slug: amazon-swf
schema_file: json-schema/amazon-swf-signalexternalworkflowexecutioninitiatedeventattributes-schema.json
slug: amazon-swf-signalexternalworkflowexecutioninitiatedeventattributes
source_filename: amazon-swf-signalexternalworkflowexecutioninitiatedeventattributes-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"required\": [\n    \"workflowId\",\n    \"signalName\",\n    \"decisionTaskCompletedEventId\"\n  ],\n  \"properties\": {\n    \"workflowId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WorkflowId\"\n        },\n        {\n          \"description\": \"The <code>workflowId</code> of the external workflow execution.\"\n        }\n      ]\n    },\n    \"runId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WorkflowRunIdOptional\"\n        },\n        {\n          \"description\": \"The <code>runId</code> of the external workflow execution to send the signal to.\"\n        }\n      ]\n    },\n    \"signalName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SignalName\"\n        },\n        {\n          \"description\": \"The name of the signal.\"\n        }\n      ]\n    },\n    \"input\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Data\"\
  \n        },\n        {\n          \"description\": \"The input provided to the signal.\"\n        }\n      ]\n    },\n    \"decisionTaskCompletedEventId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EventId\"\n        },\n        {\n          \"description\": \"The ID of the <code>DecisionTaskCompleted</code> event corresponding to the decision task that resulted in the <code>SignalExternalWorkflowExecution</code> decision for this signal. This information can be useful for diagnosing problems by tracing back the chain of events leading up to this event.\"\n        }\n      ]\n    },\n    \"control\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Data\"\n        },\n        {\n          \"description\": \"Data attached to the event that can be used by the decider in subsequent decision tasks.\"\n        }\n      ]\n    }\n  },\n  \"description\": \"Provides the details of the <code>SignalExternalWorkflowExecutionInitiated</code>\
  \ event.\",\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"SignalExternalWorkflowExecutionInitiatedEventAttributes\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-swf/refs/heads/main/json-schema/amazon-swf-signalexternalworkflowexecutioninitiatedeventattributes-schema.json
tags:
- Automation
- Task Coordination
- Workflow
title: SignalExternalWorkflowExecutionInitiatedEventAttributes
---
