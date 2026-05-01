---
description: ''
layout: schema
name: StartWorkflowExecutionInput
properties_list:
- description: ''
  name: domain
  type: object
- description: ''
  name: workflowId
  type: object
- description: ''
  name: workflowType
  type: object
- description: ''
  name: taskList
  type: object
- description: ''
  name: taskPriority
  type: object
- description: ''
  name: input
  type: object
- description: ''
  name: executionStartToCloseTimeout
  type: object
- description: ''
  name: tagList
  type: object
- description: ''
  name: taskStartToCloseTimeout
  type: object
- description: ''
  name: childPolicy
  type: object
- description: ''
  name: lambdaRole
  type: object
provider_name: Amazon Simple Workflow Service
provider_slug: amazon-swf
schema_file: json-schema/amazon-swf-startworkflowexecutioninput-schema.json
slug: amazon-swf-startworkflowexecutioninput
source_filename: amazon-swf-startworkflowexecutioninput-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"required\": [\n    \"domain\",\n    \"workflowId\",\n    \"workflowType\"\n  ],\n  \"title\": \"StartWorkflowExecutionInput\",\n  \"properties\": {\n    \"domain\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DomainName\"\n        },\n        {\n          \"description\": \"<p>The name of the domain in which the workflow execution is created.</p> <p>The specified string must not contain a <code>:</code> (colon), <code>/</code> (slash), <code>|</code> (vertical bar), or any control characters (<code>\\\\u0000-\\\\u001f</code> | <code>\\\\u007f-\\\\u009f</code>). Also, it must <i>not</i> be the literal string <code>arn</code>.</p>\"\n        }\n      ]\n    },\n    \"workflowId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WorkflowId\"\n        },\n        {\n          \"description\": \"<p>The user defined identifier associated with the workflow execution. You can use this to associate\
  \ a custom identifier with the workflow execution. You may specify the same identifier if a workflow execution is logically a <i>restart</i> of a previous execution. You cannot have two open workflow executions with the same <code>workflowId</code> at the same time within the same domain.</p> <p>The specified string must not contain a <code>:</code> (colon), <code>/</code> (slash), <code>|</code> (vertical bar), or any control characters (<code>\\\\u0000-\\\\u001f</code> | <code>\\\\u007f-\\\\u009f</code>). Also, it must <i>not</i> be the literal string <code>arn</code>.</p>\"\n        }\n      ]\n    },\n    \"workflowType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WorkflowType\"\n        },\n        {\n          \"description\": \"The type of the workflow to start.\"\n        }\n      ]\n    },\n    \"taskList\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TaskList\"\n        },\n        {\n          \"description\"\
  : \"<p>The task list to use for the decision tasks generated for this workflow execution. This overrides the <code>defaultTaskList</code> specified when registering the workflow type.</p> <note> <p>A task list for this workflow execution must be specified either as a default for the workflow type or through this parameter. If neither this parameter is set nor a default task list was specified at registration time then a fault is returned.</p> </note> <p>The specified string must not contain a <code>:</code> (colon), <code>/</code> (slash), <code>|</code> (vertical bar), or any control characters (<code>\\\\u0000-\\\\u001f</code> | <code>\\\\u007f-\\\\u009f</code>). Also, it must <i>not</i> be the literal string <code>arn</code>.</p>\"\n        }\n      ]\n    },\n    \"taskPriority\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TaskPriority\"\n        },\n        {\n          \"description\": \"<p>The task priority to use for this workflow execution. This\
  \ overrides any default priority that was assigned when the workflow type was registered. If not set, then the default task priority for the workflow type is used. Valid values are integers that range from Java's <code>Integer.MIN_VALUE</code> (-2147483648) to <code>Integer.MAX_VALUE</code> (2147483647). Higher numbers indicate higher priority.</p> <p>For more information about setting task priority, see <a href=\\\"https://docs.aws.amazon.com/amazonswf/latest/developerguide/programming-priority.html\\\">Setting Task Priority</a> in the <i>Amazon SWF Developer Guide</i>.</p>\"\n        }\n      ]\n    },\n    \"input\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Data\"\n        },\n        {\n          \"description\": \"The input for the workflow execution. This is a free form string which should be meaningful to the workflow you are starting. This <code>input</code> is made available to the new workflow execution in the <code>WorkflowExecutionStarted</code>\
  \ history event.\"\n        }\n      ]\n    },\n    \"executionStartToCloseTimeout\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DurationInSecondsOptional\"\n        },\n        {\n          \"description\": \"<p>The total duration for this workflow execution. This overrides the defaultExecutionStartToCloseTimeout specified when registering the workflow type.</p> <p>The duration is specified in seconds; an integer greater than or equal to <code>0</code>. Exceeding this limit causes the workflow execution to time out. Unlike some of the other timeout parameters in Amazon SWF, you cannot specify a value of \\\"NONE\\\" for this timeout; there is a one-year max limit on the time that a workflow execution can run.</p> <note> <p>An execution start-to-close timeout must be specified either through this parameter or as a default when the workflow type is registered. If neither this parameter nor a default execution start-to-close timeout is specified, a fault\
  \ is returned.</p> </note>\"\n        }\n      ]\n    },\n    \"tagList\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TagList\"\n        },\n        {\n          \"description\": \"The list of tags to associate with the workflow execution. You can specify a maximum of 5 tags. You can list workflow executions with a specific tag by calling <a>ListOpenWorkflowExecutions</a> or <a>ListClosedWorkflowExecutions</a> and specifying a <a>TagFilter</a>.\"\n        }\n      ]\n    },\n    \"taskStartToCloseTimeout\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DurationInSecondsOptional\"\n        },\n        {\n          \"description\": \"<p>Specifies the maximum duration of decision tasks for this workflow execution. This parameter overrides the <code>defaultTaskStartToCloseTimout</code> specified when registering the workflow type using <a>RegisterWorkflowType</a>.</p> <p>The duration is specified in seconds, an integer greater\
  \ than or equal to <code>0</code>. You can use <code>NONE</code> to specify unlimited duration.</p> <note> <p>A task start-to-close timeout for this workflow execution must be specified either as a default for the workflow type or through this parameter. If neither this parameter is set nor a default task start-to-close timeout was specified at registration time then a fault is returned.</p> </note>\"\n        }\n      ]\n    },\n    \"childPolicy\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ChildPolicy\"\n        },\n        {\n          \"description\": \"<p>If set, specifies the policy to use for the child workflow executions of this workflow execution if it is terminated, by calling the <a>TerminateWorkflowExecution</a> action explicitly or due to an expired timeout. This policy overrides the default child policy specified when registering the workflow type using <a>RegisterWorkflowType</a>.</p> <p>The supported child policies are:</p> <ul> <li> <p>\
  \ <code>TERMINATE</code> \\u2013 The child executions are terminated.</p> </li> <li> <p> <code>REQUEST_CANCEL</code> \\u2013 A request to cancel is attempted for each child execution by recording a <code>WorkflowExecutionCancelRequested</code> event in its history. It is up to the decider to take appropriate actions when it receives an execution history with this event.</p> </li> <li> <p> <code>ABANDON</code> \\u2013 No action is taken. The child executions continue to run.</p> </li> </ul> <note> <p>A child policy for this workflow execution must be specified either as a default for the workflow type or through this parameter. If neither this parameter is set nor a default child policy was specified at registration time then a fault is returned.</p> </note>\"\n        }\n      ]\n    },\n    \"lambdaRole\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Arn\"\n        },\n        {\n          \"description\": \"<p>The IAM role to attach to this workflow execution.</p>\
  \ <note> <p>Executions of this workflow type need IAM roles to invoke Lambda functions. If you don't attach an IAM role, any attempt to schedule a Lambda task fails. This results in a <code>ScheduleLambdaFunctionFailed</code> history event. For more information, see <a href=\\\"https://docs.aws.amazon.com/amazonswf/latest/developerguide/lambda-task.html\\\">https://docs.aws.amazon.com/amazonswf/latest/developerguide/lambda-task.html</a> in the <i>Amazon SWF Developer Guide</i>.</p> </note>\"\n        }\n      ]\n    }\n  },\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-swf/refs/heads/main/json-schema/amazon-swf-startworkflowexecutioninput-schema.json
tags:
- Automation
- Task Coordination
- Workflow
title: StartWorkflowExecutionInput
---
