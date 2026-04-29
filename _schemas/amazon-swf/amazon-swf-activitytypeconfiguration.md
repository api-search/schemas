---
description: Configuration settings registered with the activity type.
layout: schema
name: ActivityTypeConfiguration
properties_list:
- description: ''
  name: defaultTaskStartToCloseTimeout
  type: object
- description: ''
  name: defaultTaskHeartbeatTimeout
  type: object
- description: ''
  name: defaultTaskList
  type: object
- description: ''
  name: defaultTaskPriority
  type: object
- description: ''
  name: defaultTaskScheduleToStartTimeout
  type: object
- description: ''
  name: defaultTaskScheduleToCloseTimeout
  type: object
provider_name: Amazon Simple Workflow Service
provider_slug: amazon-swf
schema_file: json-schema/amazon-swf-activitytypeconfiguration-schema.json
slug: amazon-swf-activitytypeconfiguration
source_filename: amazon-swf-activitytypeconfiguration-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"defaultTaskStartToCloseTimeout\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DurationInSecondsOptional\"\n        },\n        {\n          \"description\": \"<p> The default maximum duration for tasks of an activity type specified when registering the activity type. You can override this default when scheduling a task through the <code>ScheduleActivityTask</code> <a>Decision</a>.</p> <p>The duration is specified in seconds, an integer greater than or equal to <code>0</code>. You can use <code>NONE</code> to specify unlimited duration.</p>\"\n        }\n      ]\n    },\n    \"defaultTaskHeartbeatTimeout\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DurationInSecondsOptional\"\n        },\n        {\n          \"description\": \"<p> The default maximum time, in seconds, before which a worker processing a task must report progress by calling <a>RecordActivityTaskHeartbeat</a>.</p>\
  \ <p>You can specify this value only when <i>registering</i> an activity type. The registered default value can be overridden when you schedule a task through the <code>ScheduleActivityTask</code> <a>Decision</a>. If the activity worker subsequently attempts to record a heartbeat or returns a result, the activity worker receives an <code>UnknownResource</code> fault. In this case, Amazon SWF no longer considers the activity task to be valid; the activity worker should clean up the activity task.</p> <p>The duration is specified in seconds, an integer greater than or equal to <code>0</code>. You can use <code>NONE</code> to specify unlimited duration.</p>\"\n        }\n      ]\n    },\n    \"defaultTaskList\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TaskList\"\n        },\n        {\n          \"description\": \" The default task list specified for this activity type at registration. This default is used if a task list isn't provided when a task is scheduled\
  \ through the <code>ScheduleActivityTask</code> <a>Decision</a>. You can override the default registered task list when scheduling a task through the <code>ScheduleActivityTask</code> <a>Decision</a>.\"\n        }\n      ]\n    },\n    \"defaultTaskPriority\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TaskPriority\"\n        },\n        {\n          \"description\": \"<p> The default task priority for tasks of this activity type, specified at registration. If not set, then <code>0</code> is used as the default priority. This default can be overridden when scheduling an activity task.</p> <p>Valid values are integers that range from Java's <code>Integer.MIN_VALUE</code> (-2147483648) to <code>Integer.MAX_VALUE</code> (2147483647). Higher numbers indicate higher priority.</p> <p>For more information about setting task priority, see <a href=\\\"https://docs.aws.amazon.com/amazonswf/latest/developerguide/programming-priority.html\\\">Setting Task Priority</a>\
  \ in the <i>Amazon SWF Developer Guide</i>.</p>\"\n        }\n      ]\n    },\n    \"defaultTaskScheduleToStartTimeout\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DurationInSecondsOptional\"\n        },\n        {\n          \"description\": \"<p> The default maximum duration, specified when registering the activity type, that a task of an activity type can wait before being assigned to a worker. You can override this default when scheduling a task through the <code>ScheduleActivityTask</code> <a>Decision</a>.</p> <p>The duration is specified in seconds, an integer greater than or equal to <code>0</code>. You can use <code>NONE</code> to specify unlimited duration.</p>\"\n        }\n      ]\n    },\n    \"defaultTaskScheduleToCloseTimeout\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DurationInSecondsOptional\"\n        },\n        {\n          \"description\": \"<p> The default maximum duration, specified when registering\
  \ the activity type, for tasks of this activity type. You can override this default when scheduling a task through the <code>ScheduleActivityTask</code> <a>Decision</a>.</p> <p>The duration is specified in seconds, an integer greater than or equal to <code>0</code>. You can use <code>NONE</code> to specify unlimited duration.</p>\"\n        }\n      ]\n    }\n  },\n  \"description\": \"Configuration settings registered with the activity type.\",\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"ActivityTypeConfiguration\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-swf/refs/heads/main/json-schema/amazon-swf-activitytypeconfiguration-schema.json
tags:
- Automation
- AWS
- Task Coordination
- Workflow
title: ActivityTypeConfiguration
---
