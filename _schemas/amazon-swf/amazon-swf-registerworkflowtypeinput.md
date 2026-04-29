---
description: ''
layout: schema
name: RegisterWorkflowTypeInput
properties_list:
- description: ''
  name: domain
  type: object
- description: ''
  name: name
  type: object
- description: ''
  name: version
  type: object
- description: ''
  name: description
  type: object
- description: ''
  name: defaultTaskStartToCloseTimeout
  type: object
- description: ''
  name: defaultExecutionStartToCloseTimeout
  type: object
- description: ''
  name: defaultTaskList
  type: object
- description: ''
  name: defaultTaskPriority
  type: object
- description: ''
  name: defaultChildPolicy
  type: object
- description: ''
  name: defaultLambdaRole
  type: object
provider_name: Amazon Simple Workflow Service
provider_slug: amazon-swf
schema_file: json-schema/amazon-swf-registerworkflowtypeinput-schema.json
slug: amazon-swf-registerworkflowtypeinput
source_filename: amazon-swf-registerworkflowtypeinput-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"required\": [\n    \"domain\",\n    \"name\",\n    \"version\"\n  ],\n  \"title\": \"RegisterWorkflowTypeInput\",\n  \"properties\": {\n    \"domain\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DomainName\"\n        },\n        {\n          \"description\": \"The name of the domain in which to register the workflow type.\"\n        }\n      ]\n    },\n    \"name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Name\"\n        },\n        {\n          \"description\": \"<p>The name of the workflow type.</p> <p>The specified string must not contain a <code>:</code> (colon), <code>/</code> (slash), <code>|</code> (vertical bar), or any control characters (<code>\\\\u0000-\\\\u001f</code> | <code>\\\\u007f-\\\\u009f</code>). Also, it must <i>not</i> be the literal string <code>arn</code>.</p>\"\n        }\n      ]\n    },\n    \"version\": {\n      \"allOf\": [\n        {\n       \
  \   \"$ref\": \"#/components/schemas/Version\"\n        },\n        {\n          \"description\": \"<p>The version of the workflow type.</p> <note> <p>The workflow type consists of the name and version, the combination of which must be unique within the domain. To get a list of all currently registered workflow types, use the <a>ListWorkflowTypes</a> action.</p> </note> <p>The specified string must not contain a <code>:</code> (colon), <code>/</code> (slash), <code>|</code> (vertical bar), or any control characters (<code>\\\\u0000-\\\\u001f</code> | <code>\\\\u007f-\\\\u009f</code>). Also, it must <i>not</i> be the literal string <code>arn</code>.</p>\"\n        }\n      ]\n    },\n    \"description\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Description\"\n        },\n        {\n          \"description\": \"Textual description of the workflow type.\"\n        }\n      ]\n    },\n    \"defaultTaskStartToCloseTimeout\": {\n      \"allOf\": [\n      \
  \  {\n          \"$ref\": \"#/components/schemas/DurationInSecondsOptional\"\n        },\n        {\n          \"description\": \"<p>If set, specifies the default maximum duration of decision tasks for this workflow type. This default can be overridden when starting a workflow execution using the <a>StartWorkflowExecution</a> action or the <code>StartChildWorkflowExecution</code> <a>Decision</a>.</p> <p>The duration is specified in seconds, an integer greater than or equal to <code>0</code>. You can use <code>NONE</code> to specify unlimited duration.</p>\"\n        }\n      ]\n    },\n    \"defaultExecutionStartToCloseTimeout\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DurationInSecondsOptional\"\n        },\n        {\n          \"description\": \"<p>If set, specifies the default maximum duration for executions of this workflow type. You can override this default when starting an execution through the <a>StartWorkflowExecution</a> Action or <code>StartChildWorkflowExecution</code>\
  \ <a>Decision</a>.</p> <p>The duration is specified in seconds; an integer greater than or equal to 0. Unlike some of the other timeout parameters in Amazon SWF, you cannot specify a value of \\\"NONE\\\" for <code>defaultExecutionStartToCloseTimeout</code>; there is a one-year max limit on the time that a workflow execution can run. Exceeding this limit always causes the workflow execution to time out.</p>\"\n        }\n      ]\n    },\n    \"defaultTaskList\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TaskList\"\n        },\n        {\n          \"description\": \"If set, specifies the default task list to use for scheduling decision tasks for executions of this workflow type. This default is used only if a task list isn't provided when starting the execution through the <a>StartWorkflowExecution</a> Action or <code>StartChildWorkflowExecution</code> <a>Decision</a>.\"\n        }\n      ]\n    },\n    \"defaultTaskPriority\": {\n      \"allOf\": [\n\
  \        {\n          \"$ref\": \"#/components/schemas/TaskPriority\"\n        },\n        {\n          \"description\": \"<p>The default task priority to assign to the workflow type. If not assigned, then <code>0</code> is used. Valid values are integers that range from Java's <code>Integer.MIN_VALUE</code> (-2147483648) to <code>Integer.MAX_VALUE</code> (2147483647). Higher numbers indicate higher priority.</p> <p>For more information about setting task priority, see <a href=\\\"https://docs.aws.amazon.com/amazonswf/latest/developerguide/programming-priority.html\\\">Setting Task Priority</a> in the <i>Amazon SWF Developer Guide</i>.</p>\"\n        }\n      ]\n    },\n    \"defaultChildPolicy\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ChildPolicy\"\n        },\n        {\n          \"description\": \"<p>If set, specifies the default policy to use for the child workflow executions when a workflow execution of this type is terminated, by calling the\
  \ <a>TerminateWorkflowExecution</a> action explicitly or due to an expired timeout. This default can be overridden when starting a workflow execution using the <a>StartWorkflowExecution</a> action or the <code>StartChildWorkflowExecution</code> <a>Decision</a>.</p> <p>The supported child policies are:</p> <ul> <li> <p> <code>TERMINATE</code> \\u2013 The child executions are terminated.</p> </li> <li> <p> <code>REQUEST_CANCEL</code> \\u2013 A request to cancel is attempted for each child execution by recording a <code>WorkflowExecutionCancelRequested</code> event in its history. It is up to the decider to take appropriate actions when it receives an execution history with this event.</p> </li> <li> <p> <code>ABANDON</code> \\u2013 No action is taken. The child executions continue to run.</p> </li> </ul>\"\n        }\n      ]\n    },\n    \"defaultLambdaRole\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Arn\"\n        },\n        {\n          \"description\"\
  : \"<p>The default IAM role attached to this workflow type.</p> <note> <p>Executions of this workflow type need IAM roles to invoke Lambda functions. If you don't specify an IAM role when you start this workflow type, the default Lambda role is attached to the execution. For more information, see <a href=\\\"https://docs.aws.amazon.com/amazonswf/latest/developerguide/lambda-task.html\\\">https://docs.aws.amazon.com/amazonswf/latest/developerguide/lambda-task.html</a> in the <i>Amazon SWF Developer Guide</i>.</p> </note>\"\n        }\n      ]\n    }\n  },\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-swf/refs/heads/main/json-schema/amazon-swf-registerworkflowtypeinput-schema.json
tags:
- Automation
- AWS
- Task Coordination
- Workflow
title: RegisterWorkflowTypeInput
---
