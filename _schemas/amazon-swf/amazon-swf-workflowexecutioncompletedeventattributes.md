---
description: Provides the details of the <code>WorkflowExecutionCompleted</code> event.
layout: schema
name: WorkflowExecutionCompletedEventAttributes
properties_list:
- description: ''
  name: result
  type: object
- description: ''
  name: decisionTaskCompletedEventId
  type: object
provider_name: Amazon Simple Workflow Service
provider_slug: amazon-swf
schema_file: json-schema/amazon-swf-workflowexecutioncompletedeventattributes-schema.json
slug: amazon-swf-workflowexecutioncompletedeventattributes
source_filename: amazon-swf-workflowexecutioncompletedeventattributes-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"required\": [\n    \"decisionTaskCompletedEventId\"\n  ],\n  \"properties\": {\n    \"result\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Data\"\n        },\n        {\n          \"description\": \"The result produced by the workflow execution upon successful completion.\"\n        }\n      ]\n    },\n    \"decisionTaskCompletedEventId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EventId\"\n        },\n        {\n          \"description\": \"The ID of the <code>DecisionTaskCompleted</code> event corresponding to the decision task that resulted in the <code>CompleteWorkflowExecution</code> decision to complete this execution. This information can be useful for diagnosing problems by tracing back the chain of events leading up to this event.\"\n        }\n      ]\n    }\n  },\n  \"description\": \"Provides the details of the <code>WorkflowExecutionCompleted</code> event.\",\n\
  \  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"WorkflowExecutionCompletedEventAttributes\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-swf/refs/heads/main/json-schema/amazon-swf-workflowexecutioncompletedeventattributes-schema.json
tags:
- Automation
- AWS
- Task Coordination
- Workflow
title: WorkflowExecutionCompletedEventAttributes
---
