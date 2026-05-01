---
description: The configuration settings for a workflow execution including timeout values, tasklist etc. These configuration settings are determined from the defaults specified when registering the workflow type and those specified when starting the workflow execution.
layout: schema
name: WorkflowExecutionConfiguration
properties_list:
- description: ''
  name: taskStartToCloseTimeout
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
  name: childPolicy
  type: object
- description: ''
  name: lambdaRole
  type: object
provider_name: Amazon Simple Workflow Service
provider_slug: amazon-swf
schema_file: json-schema/amazon-swf-workflowexecutionconfiguration-schema.json
slug: amazon-swf-workflowexecutionconfiguration
source_filename: amazon-swf-workflowexecutionconfiguration-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"required\": [\n    \"taskStartToCloseTimeout\",\n    \"executionStartToCloseTimeout\",\n    \"taskList\",\n    \"childPolicy\"\n  ],\n  \"properties\": {\n    \"taskStartToCloseTimeout\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DurationInSeconds\"\n        },\n        {\n          \"description\": \"<p>The maximum duration allowed for decision tasks for this workflow execution.</p> <p>The duration is specified in seconds, an integer greater than or equal to <code>0</code>. You can use <code>NONE</code> to specify unlimited duration.</p>\"\n        }\n      ]\n    },\n    \"executionStartToCloseTimeout\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DurationInSeconds\"\n        },\n        {\n          \"description\": \"<p>The total duration for this workflow execution.</p> <p>The duration is specified in seconds, an integer greater than or equal to <code>0</code>. You can use\
  \ <code>NONE</code> to specify unlimited duration.</p>\"\n        }\n      ]\n    },\n    \"taskList\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TaskList\"\n        },\n        {\n          \"description\": \"The task list used for the decision tasks generated for this workflow execution.\"\n        }\n      ]\n    },\n    \"taskPriority\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TaskPriority\"\n        },\n        {\n          \"description\": \"<p>The priority assigned to decision tasks for this workflow execution. Valid values are integers that range from Java's <code>Integer.MIN_VALUE</code> (-2147483648) to <code>Integer.MAX_VALUE</code> (2147483647). Higher numbers indicate higher priority.</p> <p>For more information about setting task priority, see <a href=\\\"https://docs.aws.amazon.com/amazonswf/latest/developerguide/programming-priority.html\\\">Setting Task Priority</a> in the <i>Amazon SWF Developer Guide</i>.</p>\"\
  \n        }\n      ]\n    },\n    \"childPolicy\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ChildPolicy\"\n        },\n        {\n          \"description\": \"<p>The policy to use for the child workflow executions if this workflow execution is terminated, by calling the <a>TerminateWorkflowExecution</a> action explicitly or due to an expired timeout.</p> <p>The supported child policies are:</p> <ul> <li> <p> <code>TERMINATE</code> \\u2013 The child executions are terminated.</p> </li> <li> <p> <code>REQUEST_CANCEL</code> \\u2013 A request to cancel is attempted for each child execution by recording a <code>WorkflowExecutionCancelRequested</code> event in its history. It is up to the decider to take appropriate actions when it receives an execution history with this event.</p> </li> <li> <p> <code>ABANDON</code> \\u2013 No action is taken. The child executions continue to run.</p> </li> </ul>\"\n        }\n      ]\n    },\n    \"lambdaRole\": {\n    \
  \  \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Arn\"\n        },\n        {\n          \"description\": \"The IAM role attached to the child workflow execution.\"\n        }\n      ]\n    }\n  },\n  \"description\": \"The configuration settings for a workflow execution including timeout values, tasklist etc. These configuration settings are determined from the defaults specified when registering the workflow type and those specified when starting the workflow execution.\",\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"WorkflowExecutionConfiguration\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-swf/refs/heads/main/json-schema/amazon-swf-workflowexecutionconfiguration-schema.json
tags:
- Automation
- Task Coordination
- Workflow
title: WorkflowExecutionConfiguration
---
