---
description: Contains information about a workflow execution.
layout: schema
name: WorkflowExecutionInfo
properties_list:
- description: ''
  name: execution
  type: object
- description: ''
  name: workflowType
  type: object
- description: ''
  name: startTimestamp
  type: object
- description: ''
  name: closeTimestamp
  type: object
- description: ''
  name: executionStatus
  type: object
- description: ''
  name: closeStatus
  type: object
- description: ''
  name: parent
  type: object
- description: ''
  name: tagList
  type: object
- description: ''
  name: cancelRequested
  type: object
provider_name: Amazon Simple Workflow Service
provider_slug: amazon-swf
schema_file: json-schema/amazon-swf-workflowexecutioninfo-schema.json
slug: amazon-swf-workflowexecutioninfo
source_json: "{\n  \"type\": \"object\",\n  \"required\": [\n    \"execution\",\n    \"workflowType\",\n    \"startTimestamp\",\n    \"executionStatus\"\n  ],\n  \"properties\": {\n    \"execution\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WorkflowExecution\"\n        },\n        {\n          \"description\": \"The workflow execution this information is about.\"\n        }\n      ]\n    },\n    \"workflowType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WorkflowType\"\n        },\n        {\n          \"description\": \"The type of the workflow execution.\"\n        }\n      ]\n    },\n    \"startTimestamp\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The time when the execution was started.\"\n        }\n      ]\n    },\n    \"closeTimestamp\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\
  \n        },\n        {\n          \"description\": \"The time when the workflow execution was closed. Set only if the execution status is CLOSED.\"\n        }\n      ]\n    },\n    \"executionStatus\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ExecutionStatus\"\n        },\n        {\n          \"description\": \"The current status of the execution.\"\n        }\n      ]\n    },\n    \"closeStatus\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CloseStatus\"\n        },\n        {\n          \"description\": \"<p>If the execution status is closed then this specifies how the execution was closed:</p> <ul> <li> <p> <code>COMPLETED</code> \\u2013 the execution was successfully completed.</p> </li> <li> <p> <code>CANCELED</code> \\u2013 the execution was canceled.Cancellation allows the implementation to gracefully clean up before the execution is closed.</p> </li> <li> <p> <code>TERMINATED</code> \\u2013 the execution was\
  \ force terminated.</p> </li> <li> <p> <code>FAILED</code> \\u2013 the execution failed to complete.</p> </li> <li> <p> <code>TIMED_OUT</code> \\u2013 the execution did not complete in the alloted time and was automatically timed out.</p> </li> <li> <p> <code>CONTINUED_AS_NEW</code> \\u2013 the execution is logically continued. This means the current execution was completed and a new execution was started to carry on the workflow.</p> </li> </ul>\"\n        }\n      ]\n    },\n    \"parent\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WorkflowExecution\"\n        },\n        {\n          \"description\": \"If this workflow execution is a child of another execution then contains the workflow execution that started this execution.\"\n        }\n      ]\n    },\n    \"tagList\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TagList\"\n        },\n        {\n          \"description\": \"The list of tags associated with the workflow\
  \ execution. Tags can be used to identify and list workflow executions of interest through the visibility APIs. A workflow execution can have a maximum of 5 tags.\"\n        }\n      ]\n    },\n    \"cancelRequested\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Canceled\"\n        },\n        {\n          \"description\": \"Set to true if a cancellation is requested for this workflow execution.\"\n        }\n      ]\n    }\n  },\n  \"description\": \"Contains information about a workflow execution.\",\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"WorkflowExecutionInfo\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-swf/refs/heads/main/json-schema/amazon-swf-workflowexecutioninfo-schema.json
tags:
- Automation
- AWS
- Task Coordination
- Workflow
title: WorkflowExecutionInfo
---
