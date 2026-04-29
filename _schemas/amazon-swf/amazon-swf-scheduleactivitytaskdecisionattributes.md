---
description: <p>Provides the details of the <code>ScheduleActivityTask</code> decision.</p> <p> <b>Access Control</b> </p> <p>You can use IAM policies to control this decision's access to Amazon SWF resources as follows:</p> <ul> <li> <p>Use a <code>Resource</code> element with the domain name to limit the action to only specified domains.</p> </li> <li> <p>Use an <code>Action</code> element to allow or deny permission to call this action.</p> </li> <li> <p>Constrain the following parameters by using a <code>Condition</code> element with the appropriate keys.</p> <ul> <li> <p> <code>activityType.name</code> – String constraint. The key is <code>swf:activityType.name</code>.</p> </li> <li> <p> <code>activityType.version</code> – String constraint. The key is <code>swf:activityType.version</code>.</p> </li> <li> <p> <code>taskList</code> – String constraint. The key is <code>swf:taskList.name</code>.</p> </li> </ul> </li> </ul> <p>If the caller doesn't have sufficient permissions to invoke
  the action, or the parameter values fall outside the specified constraints, the action fails. The associated event attribute's <code>cause</code> parameter is set to <code>OPERATION_NOT_PERMITTED</code>. For details and example IAM policies, see <a href="https://docs.aws.amazon.com/amazonswf/latest/developerguide/swf-dev-iam.html">Using IAM to Manage Access to Amazon SWF Workflows</a> in the <i>Amazon SWF Developer Guide</i>.</p>
layout: schema
name: ScheduleActivityTaskDecisionAttributes
properties_list:
- description: ''
  name: activityType
  type: object
- description: ''
  name: activityId
  type: object
- description: ''
  name: control
  type: object
- description: ''
  name: input
  type: object
- description: ''
  name: scheduleToCloseTimeout
  type: object
- description: ''
  name: taskList
  type: object
- description: ''
  name: taskPriority
  type: object
- description: ''
  name: scheduleToStartTimeout
  type: object
- description: ''
  name: startToCloseTimeout
  type: object
- description: ''
  name: heartbeatTimeout
  type: object
provider_name: Amazon Simple Workflow Service
provider_slug: amazon-swf
schema_file: json-schema/amazon-swf-scheduleactivitytaskdecisionattributes-schema.json
slug: amazon-swf-scheduleactivitytaskdecisionattributes
source_json: "{\n  \"type\": \"object\",\n  \"required\": [\n    \"activityType\",\n    \"activityId\"\n  ],\n  \"properties\": {\n    \"activityType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ActivityType\"\n        },\n        {\n          \"description\": \" The type of the activity task to schedule.\"\n        }\n      ]\n    },\n    \"activityId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ActivityId\"\n        },\n        {\n          \"description\": \"<p> The <code>activityId</code> of the activity task.</p> <p>The specified string must not contain a <code>:</code> (colon), <code>/</code> (slash), <code>|</code> (vertical bar), or any control characters (<code>\\\\u0000-\\\\u001f</code> | <code>\\\\u007f-\\\\u009f</code>). Also, it must <i>not</i> be the literal string <code>arn</code>.</p>\"\n        }\n      ]\n    },\n    \"control\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Data\"\
  \n        },\n        {\n          \"description\": \"Data attached to the event that can be used by the decider in subsequent workflow tasks. This data isn't sent to the activity.\"\n        }\n      ]\n    },\n    \"input\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Data\"\n        },\n        {\n          \"description\": \"The input provided to the activity task.\"\n        }\n      ]\n    },\n    \"scheduleToCloseTimeout\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DurationInSecondsOptional\"\n        },\n        {\n          \"description\": \"<p>The maximum duration for this activity task.</p> <p>The duration is specified in seconds, an integer greater than or equal to <code>0</code>. You can use <code>NONE</code> to specify unlimited duration.</p> <note> <p>A schedule-to-close timeout for this activity task must be specified either as a default for the activity type or through this field. If neither this field\
  \ is set nor a default schedule-to-close timeout was specified at registration time then a fault is returned.</p> </note>\"\n        }\n      ]\n    },\n    \"taskList\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TaskList\"\n        },\n        {\n          \"description\": \"<p>If set, specifies the name of the task list in which to schedule the activity task. If not specified, the <code>defaultTaskList</code> registered with the activity type is used.</p> <note> <p>A task list for this activity task must be specified either as a default for the activity type or through this field. If neither this field is set nor a default task list was specified at registration time then a fault is returned.</p> </note> <p>The specified string must not contain a <code>:</code> (colon), <code>/</code> (slash), <code>|</code> (vertical bar), or any control characters (<code>\\\\u0000-\\\\u001f</code> | <code>\\\\u007f-\\\\u009f</code>). Also, it must <i>not</i> be the\
  \ literal string <code>arn</code>.</p>\"\n        }\n      ]\n    },\n    \"taskPriority\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TaskPriority\"\n        },\n        {\n          \"description\": \"<p> If set, specifies the priority with which the activity task is to be assigned to a worker. This overrides the defaultTaskPriority specified when registering the activity type using <a>RegisterActivityType</a>. Valid values are integers that range from Java's <code>Integer.MIN_VALUE</code> (-2147483648) to <code>Integer.MAX_VALUE</code> (2147483647). Higher numbers indicate higher priority.</p> <p>For more information about setting task priority, see <a href=\\\"https://docs.aws.amazon.com/amazonswf/latest/developerguide/programming-priority.html\\\">Setting Task Priority</a> in the <i>Amazon SWF Developer Guide</i>.</p>\"\n        }\n      ]\n    },\n    \"scheduleToStartTimeout\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DurationInSecondsOptional\"\
  \n        },\n        {\n          \"description\": \"<p> If set, specifies the maximum duration the activity task can wait to be assigned to a worker. This overrides the default schedule-to-start timeout specified when registering the activity type using <a>RegisterActivityType</a>.</p> <p>The duration is specified in seconds, an integer greater than or equal to <code>0</code>. You can use <code>NONE</code> to specify unlimited duration.</p> <note> <p>A schedule-to-start timeout for this activity task must be specified either as a default for the activity type or through this field. If neither this field is set nor a default schedule-to-start timeout was specified at registration time then a fault is returned.</p> </note>\"\n        }\n      ]\n    },\n    \"startToCloseTimeout\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DurationInSecondsOptional\"\n        },\n        {\n          \"description\": \"<p>If set, specifies the maximum duration a worker\
  \ may take to process this activity task. This overrides the default start-to-close timeout specified when registering the activity type using <a>RegisterActivityType</a>.</p> <p>The duration is specified in seconds, an integer greater than or equal to <code>0</code>. You can use <code>NONE</code> to specify unlimited duration.</p> <note> <p>A start-to-close timeout for this activity task must be specified either as a default for the activity type or through this field. If neither this field is set nor a default start-to-close timeout was specified at registration time then a fault is returned.</p> </note>\"\n        }\n      ]\n    },\n    \"heartbeatTimeout\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DurationInSecondsOptional\"\n        },\n        {\n          \"description\": \"<p>If set, specifies the maximum time before which a worker processing a task of this type must report progress by calling <a>RecordActivityTaskHeartbeat</a>. If the timeout\
  \ is exceeded, the activity task is automatically timed out. If the worker subsequently attempts to record a heartbeat or returns a result, it is ignored. This overrides the default heartbeat timeout specified when registering the activity type using <a>RegisterActivityType</a>.</p> <p>The duration is specified in seconds, an integer greater than or equal to <code>0</code>. You can use <code>NONE</code> to specify unlimited duration.</p>\"\n        }\n      ]\n    }\n  },\n  \"description\": \"<p>Provides the details of the <code>ScheduleActivityTask</code> decision.</p> <p> <b>Access Control</b> </p> <p>You can use IAM policies to control this decision's access to Amazon SWF resources as follows:</p> <ul> <li> <p>Use a <code>Resource</code> element with the domain name to limit the action to only specified domains.</p> </li> <li> <p>Use an <code>Action</code> element to allow or deny permission to call this action.</p> </li> <li> <p>Constrain the following parameters by using a <code>Condition</code>\
  \ element with the appropriate keys.</p> <ul> <li> <p> <code>activityType.name</code> \\u2013 String constraint. The key is <code>swf:activityType.name</code>.</p> </li> <li> <p> <code>activityType.version</code> \\u2013 String constraint. The key is <code>swf:activityType.version</code>.</p> </li> <li> <p> <code>taskList</code> \\u2013 String constraint. The key is <code>swf:taskList.name</code>.</p> </li> </ul> </li> </ul> <p>If the caller doesn't have sufficient permissions to invoke the action, or the parameter values fall outside the specified constraints, the action fails. The associated event attribute's <code>cause</code> parameter is set to <code>OPERATION_NOT_PERMITTED</code>. For details and example IAM policies, see <a href=\\\"https://docs.aws.amazon.com/amazonswf/latest/developerguide/swf-dev-iam.html\\\">Using IAM to Manage Access to Amazon SWF Workflows</a> in the <i>Amazon SWF Developer Guide</i>.</p>\",\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"\
  title\": \"ScheduleActivityTaskDecisionAttributes\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-swf/refs/heads/main/json-schema/amazon-swf-scheduleactivitytaskdecisionattributes-schema.json
tags:
- Automation
- AWS
- Task Coordination
- Workflow
title: ScheduleActivityTaskDecisionAttributes
---
