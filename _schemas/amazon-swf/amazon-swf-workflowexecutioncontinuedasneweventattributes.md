---
description: Provides the details of the <code>WorkflowExecutionContinuedAsNew</code> event.
layout: schema
name: WorkflowExecutionContinuedAsNewEventAttributes
properties_list:
- description: ''
  name: input
  type: object
- description: ''
  name: decisionTaskCompletedEventId
  type: object
- description: ''
  name: newExecutionRunId
  type: object
- description: ''
  name: executionStartToCloseTimeout
  type: object
- description: ''
  name: taskList
  type: object
- description: ''
  name: taskPriority
  type: object
- description: ''
  name: taskStartToCloseTimeout
  type: object
- description: ''
  name: childPolicy
  type: object
- description: ''
  name: tagList
  type: object
- description: ''
  name: workflowType
  type: object
- description: ''
  name: lambdaRole
  type: object
provider_name: Amazon Simple Workflow Service
provider_slug: amazon-swf
schema_file: json-schema/amazon-swf-workflowexecutioncontinuedasneweventattributes-schema.json
slug: amazon-swf-workflowexecutioncontinuedasneweventattributes
source_json: "{\n  \"type\": \"object\",\n  \"required\": [\n    \"decisionTaskCompletedEventId\",\n    \"newExecutionRunId\",\n    \"taskList\",\n    \"childPolicy\",\n    \"workflowType\"\n  ],\n  \"properties\": {\n    \"input\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Data\"\n        },\n        {\n          \"description\": \"The input provided to the new workflow execution.\"\n        }\n      ]\n    },\n    \"decisionTaskCompletedEventId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EventId\"\n        },\n        {\n          \"description\": \"The ID of the <code>DecisionTaskCompleted</code> event corresponding to the decision task that resulted in the <code>ContinueAsNewWorkflowExecution</code> decision that started this execution. This information can be useful for diagnosing problems by tracing back the chain of events leading up to this event.\"\n        }\n      ]\n    },\n    \"newExecutionRunId\": {\n \
  \     \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WorkflowRunId\"\n        },\n        {\n          \"description\": \"The <code>runId</code> of the new workflow execution.\"\n        }\n      ]\n    },\n    \"executionStartToCloseTimeout\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DurationInSecondsOptional\"\n        },\n        {\n          \"description\": \"<p>The total duration allowed for the new workflow execution.</p> <p>The duration is specified in seconds, an integer greater than or equal to <code>0</code>. You can use <code>NONE</code> to specify unlimited duration.</p>\"\n        }\n      ]\n    },\n    \"taskList\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TaskList\"\n        },\n        {\n          \"description\": \"The task list to use for the decisions of the new (continued) workflow execution.\"\n        }\n      ]\n    },\n    \"taskPriority\": {\n      \"allOf\": [\n   \
  \     {\n          \"$ref\": \"#/components/schemas/TaskPriority\"\n        },\n        {\n          \"description\": \"The priority of the task to use for the decisions of the new (continued) workflow execution.\"\n        }\n      ]\n    },\n    \"taskStartToCloseTimeout\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DurationInSecondsOptional\"\n        },\n        {\n          \"description\": \"<p>The maximum duration of decision tasks for the new workflow execution.</p> <p>The duration is specified in seconds, an integer greater than or equal to <code>0</code>. You can use <code>NONE</code> to specify unlimited duration.</p>\"\n        }\n      ]\n    },\n    \"childPolicy\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ChildPolicy\"\n        },\n        {\n          \"description\": \"<p>The policy to use for the child workflow executions of the new execution if it is terminated by calling the <a>TerminateWorkflowExecution</a>\
  \ action explicitly or due to an expired timeout.</p> <p>The supported child policies are:</p> <ul> <li> <p> <code>TERMINATE</code> \\u2013 The child executions are terminated.</p> </li> <li> <p> <code>REQUEST_CANCEL</code> \\u2013 A request to cancel is attempted for each child execution by recording a <code>WorkflowExecutionCancelRequested</code> event in its history. It is up to the decider to take appropriate actions when it receives an execution history with this event.</p> </li> <li> <p> <code>ABANDON</code> \\u2013 No action is taken. The child executions continue to run.</p> </li> </ul>\"\n        }\n      ]\n    },\n    \"tagList\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TagList\"\n        },\n        {\n          \"description\": \"The list of tags associated with the new workflow execution.\"\n        }\n      ]\n    },\n    \"workflowType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WorkflowType\"\n  \
  \      },\n        {\n          \"description\": \"The workflow type of this execution.\"\n        }\n      ]\n    },\n    \"lambdaRole\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Arn\"\n        },\n        {\n          \"description\": \"The IAM role to attach to the new (continued) workflow execution.\"\n        }\n      ]\n    }\n  },\n  \"description\": \"Provides the details of the <code>WorkflowExecutionContinuedAsNew</code> event.\",\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"WorkflowExecutionContinuedAsNewEventAttributes\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-swf/refs/heads/main/json-schema/amazon-swf-workflowexecutioncontinuedasneweventattributes-schema.json
tags:
- Automation
- AWS
- Task Coordination
- Workflow
title: WorkflowExecutionContinuedAsNewEventAttributes
---
