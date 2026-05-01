---
description: Provides the details of the <code>StartChildWorkflowExecutionInitiated</code> event.
layout: schema
name: StartChildWorkflowExecutionInitiatedEventAttributes
properties_list:
- description: ''
  name: workflowId
  type: object
- description: ''
  name: workflowType
  type: object
- description: ''
  name: control
  type: object
- description: ''
  name: input
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
  name: decisionTaskCompletedEventId
  type: object
- description: ''
  name: childPolicy
  type: object
- description: ''
  name: taskStartToCloseTimeout
  type: object
- description: ''
  name: tagList
  type: object
- description: ''
  name: lambdaRole
  type: object
provider_name: Amazon Simple Workflow Service
provider_slug: amazon-swf
schema_file: json-schema/amazon-swf-startchildworkflowexecutioninitiatedeventattributes-schema.json
slug: amazon-swf-startchildworkflowexecutioninitiatedeventattributes
source_filename: amazon-swf-startchildworkflowexecutioninitiatedeventattributes-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"required\": [\n    \"workflowId\",\n    \"workflowType\",\n    \"taskList\",\n    \"decisionTaskCompletedEventId\",\n    \"childPolicy\"\n  ],\n  \"properties\": {\n    \"workflowId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WorkflowId\"\n        },\n        {\n          \"description\": \"The <code>workflowId</code> of the child workflow execution.\"\n        }\n      ]\n    },\n    \"workflowType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WorkflowType\"\n        },\n        {\n          \"description\": \"The type of the child workflow execution.\"\n        }\n      ]\n    },\n    \"control\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Data\"\n        },\n        {\n          \"description\": \"Data attached to the event that can be used by the decider in subsequent decision tasks. This data isn't sent to the activity.\"\n        }\n\
  \      ]\n    },\n    \"input\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Data\"\n        },\n        {\n          \"description\": \"The inputs provided to the child workflow execution.\"\n        }\n      ]\n    },\n    \"executionStartToCloseTimeout\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DurationInSecondsOptional\"\n        },\n        {\n          \"description\": \"<p>The maximum duration for the child workflow execution. If the workflow execution isn't closed within this duration, it is timed out and force-terminated.</p> <p>The duration is specified in seconds, an integer greater than or equal to <code>0</code>. You can use <code>NONE</code> to specify unlimited duration.</p>\"\n        }\n      ]\n    },\n    \"taskList\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TaskList\"\n        },\n        {\n          \"description\": \"The name of the task list used for the decision\
  \ tasks of the child workflow execution.\"\n        }\n      ]\n    },\n    \"taskPriority\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TaskPriority\"\n        },\n        {\n          \"description\": \"<p> The priority assigned for the decision tasks for this workflow execution. Valid values are integers that range from Java's <code>Integer.MIN_VALUE</code> (-2147483648) to <code>Integer.MAX_VALUE</code> (2147483647). Higher numbers indicate higher priority.</p> <p>For more information about setting task priority, see <a href=\\\"https://docs.aws.amazon.com/amazonswf/latest/developerguide/programming-priority.html\\\">Setting Task Priority</a> in the <i>Amazon SWF Developer Guide</i>.</p>\"\n        }\n      ]\n    },\n    \"decisionTaskCompletedEventId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EventId\"\n        },\n        {\n          \"description\": \"The ID of the <code>DecisionTaskCompleted</code> event corresponding\
  \ to the decision task that resulted in the <code>StartChildWorkflowExecution</code> <a>Decision</a> to request this child workflow execution. This information can be useful for diagnosing problems by tracing back the cause of events.\"\n        }\n      ]\n    },\n    \"childPolicy\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ChildPolicy\"\n        },\n        {\n          \"description\": \"<p>The policy to use for the child workflow executions if this execution gets terminated by explicitly calling the <a>TerminateWorkflowExecution</a> action or due to an expired timeout.</p> <p>The supported child policies are:</p> <ul> <li> <p> <code>TERMINATE</code> \\u2013 The child executions are terminated.</p> </li> <li> <p> <code>REQUEST_CANCEL</code> \\u2013 A request to cancel is attempted for each child execution by recording a <code>WorkflowExecutionCancelRequested</code> event in its history. It is up to the decider to take appropriate actions when it\
  \ receives an execution history with this event.</p> </li> <li> <p> <code>ABANDON</code> \\u2013 No action is taken. The child executions continue to run.</p> </li> </ul>\"\n        }\n      ]\n    },\n    \"taskStartToCloseTimeout\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DurationInSecondsOptional\"\n        },\n        {\n          \"description\": \"<p>The maximum duration allowed for the decision tasks for this workflow execution.</p> <p>The duration is specified in seconds, an integer greater than or equal to <code>0</code>. You can use <code>NONE</code> to specify unlimited duration.</p>\"\n        }\n      ]\n    },\n    \"tagList\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TagList\"\n        },\n        {\n          \"description\": \"The list of tags to associated with the child workflow execution.\"\n        }\n      ]\n    },\n    \"lambdaRole\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"\
  #/components/schemas/Arn\"\n        },\n        {\n          \"description\": \"The IAM role to attach to the child workflow execution.\"\n        }\n      ]\n    }\n  },\n  \"description\": \"Provides the details of the <code>StartChildWorkflowExecutionInitiated</code> event.\",\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"StartChildWorkflowExecutionInitiatedEventAttributes\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-swf/refs/heads/main/json-schema/amazon-swf-startchildworkflowexecutioninitiatedeventattributes-schema.json
tags:
- Automation
- Task Coordination
- Workflow
title: StartChildWorkflowExecutionInitiatedEventAttributes
---
