---
description: Provides details of <code>WorkflowExecutionStarted</code> event.
layout: schema
name: WorkflowExecutionStartedEventAttributes
properties_list:
- description: ''
  name: input
  type: object
- description: ''
  name: executionStartToCloseTimeout
  type: object
- description: ''
  name: taskStartToCloseTimeout
  type: object
- description: ''
  name: childPolicy
  type: object
- description: ''
  name: taskList
  type: object
- description: ''
  name: taskPriority
  type: object
- description: ''
  name: workflowType
  type: object
- description: ''
  name: tagList
  type: object
- description: ''
  name: continuedExecutionRunId
  type: object
- description: ''
  name: parentWorkflowExecution
  type: object
- description: ''
  name: parentInitiatedEventId
  type: object
- description: ''
  name: lambdaRole
  type: object
provider_name: Amazon Simple Workflow Service
provider_slug: amazon-swf
schema_file: json-schema/amazon-swf-workflowexecutionstartedeventattributes-schema.json
slug: amazon-swf-workflowexecutionstartedeventattributes
source_json: "{\n  \"type\": \"object\",\n  \"required\": [\n    \"childPolicy\",\n    \"taskList\",\n    \"workflowType\"\n  ],\n  \"properties\": {\n    \"input\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Data\"\n        },\n        {\n          \"description\": \"The input provided to the workflow execution.\"\n        }\n      ]\n    },\n    \"executionStartToCloseTimeout\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DurationInSecondsOptional\"\n        },\n        {\n          \"description\": \"<p>The maximum duration for this workflow execution.</p> <p>The duration is specified in seconds, an integer greater than or equal to <code>0</code>. You can use <code>NONE</code> to specify unlimited duration.</p>\"\n        }\n      ]\n    },\n    \"taskStartToCloseTimeout\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DurationInSecondsOptional\"\n        },\n        {\n          \"description\"\
  : \"<p>The maximum duration of decision tasks for this workflow type.</p> <p>The duration is specified in seconds, an integer greater than or equal to <code>0</code>. You can use <code>NONE</code> to specify unlimited duration.</p>\"\n        }\n      ]\n    },\n    \"childPolicy\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ChildPolicy\"\n        },\n        {\n          \"description\": \"<p>The policy to use for the child workflow executions if this workflow execution is terminated, by calling the <a>TerminateWorkflowExecution</a> action explicitly or due to an expired timeout.</p> <p>The supported child policies are:</p> <ul> <li> <p> <code>TERMINATE</code> \\u2013 The child executions are terminated.</p> </li> <li> <p> <code>REQUEST_CANCEL</code> \\u2013 A request to cancel is attempted for each child execution by recording a <code>WorkflowExecutionCancelRequested</code> event in its history. It is up to the decider to take appropriate actions when\
  \ it receives an execution history with this event.</p> </li> <li> <p> <code>ABANDON</code> \\u2013 No action is taken. The child executions continue to run.</p> </li> </ul>\"\n        }\n      ]\n    },\n    \"taskList\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TaskList\"\n        },\n        {\n          \"description\": \"The name of the task list for scheduling the decision tasks for this workflow execution.\"\n        }\n      ]\n    },\n    \"taskPriority\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TaskPriority\"\n        },\n        {\n          \"description\": \"The priority of the decision tasks in the workflow execution.\"\n        }\n      ]\n    },\n    \"workflowType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WorkflowType\"\n        },\n        {\n          \"description\": \"The workflow type of this execution.\"\n        }\n      ]\n    },\n    \"tagList\": {\n\
  \      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TagList\"\n        },\n        {\n          \"description\": \"The list of tags associated with this workflow execution. An execution can have up to 5 tags.\"\n        }\n      ]\n    },\n    \"continuedExecutionRunId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WorkflowRunIdOptional\"\n        },\n        {\n          \"description\": \"If this workflow execution was started due to a <code>ContinueAsNewWorkflowExecution</code> decision, then it contains the <code>runId</code> of the previous workflow execution that was closed and continued as this execution.\"\n        }\n      ]\n    },\n    \"parentWorkflowExecution\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WorkflowExecution\"\n        },\n        {\n          \"description\": \"The source workflow execution that started this workflow execution. The member isn't set if the workflow execution\
  \ was not started by a workflow.\"\n        }\n      ]\n    },\n    \"parentInitiatedEventId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EventId\"\n        },\n        {\n          \"description\": \"The ID of the <code>StartChildWorkflowExecutionInitiated</code> event corresponding to the <code>StartChildWorkflowExecution</code> <a>Decision</a> to start this workflow execution. The source event with this ID can be found in the history of the source workflow execution. This information can be useful for diagnosing problems by tracing back the chain of events leading up to this event.\"\n        }\n      ]\n    },\n    \"lambdaRole\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Arn\"\n        },\n        {\n          \"description\": \"The IAM role attached to the workflow execution.\"\n        }\n      ]\n    }\n  },\n  \"description\": \"Provides details of <code>WorkflowExecutionStarted</code> event.\",\n  \"$schema\"\
  : \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"WorkflowExecutionStartedEventAttributes\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-swf/refs/heads/main/json-schema/amazon-swf-workflowexecutionstartedeventattributes-schema.json
tags:
- Automation
- AWS
- Task Coordination
- Workflow
title: WorkflowExecutionStartedEventAttributes
---
