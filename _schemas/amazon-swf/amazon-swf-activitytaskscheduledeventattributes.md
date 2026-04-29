---
description: Provides the details of the <code>ActivityTaskScheduled</code> event.
layout: schema
name: ActivityTaskScheduledEventAttributes
properties_list:
- description: ''
  name: activityType
  type: object
- description: ''
  name: activityId
  type: object
- description: ''
  name: input
  type: object
- description: ''
  name: control
  type: object
- description: ''
  name: scheduleToStartTimeout
  type: object
- description: ''
  name: scheduleToCloseTimeout
  type: object
- description: ''
  name: startToCloseTimeout
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
  name: heartbeatTimeout
  type: object
provider_name: Amazon Simple Workflow Service
provider_slug: amazon-swf
schema_file: json-schema/amazon-swf-activitytaskscheduledeventattributes-schema.json
slug: amazon-swf-activitytaskscheduledeventattributes
source_json: "{\n  \"type\": \"object\",\n  \"required\": [\n    \"activityType\",\n    \"activityId\",\n    \"taskList\",\n    \"decisionTaskCompletedEventId\"\n  ],\n  \"properties\": {\n    \"activityType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ActivityType\"\n        },\n        {\n          \"description\": \"The type of the activity task.\"\n        }\n      ]\n    },\n    \"activityId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ActivityId\"\n        },\n        {\n          \"description\": \"The unique ID of the activity task.\"\n        }\n      ]\n    },\n    \"input\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Data\"\n        },\n        {\n          \"description\": \"The input provided to the activity task.\"\n        }\n      ]\n    },\n    \"control\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Data\"\n        },\n        {\n    \
  \      \"description\": \"Data attached to the event that can be used by the decider in subsequent workflow tasks. This data isn't sent to the activity.\"\n        }\n      ]\n    },\n    \"scheduleToStartTimeout\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DurationInSecondsOptional\"\n        },\n        {\n          \"description\": \"The maximum amount of time the activity task can wait to be assigned to a worker.\"\n        }\n      ]\n    },\n    \"scheduleToCloseTimeout\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DurationInSecondsOptional\"\n        },\n        {\n          \"description\": \"The maximum amount of time for this activity task.\"\n        }\n      ]\n    },\n    \"startToCloseTimeout\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DurationInSecondsOptional\"\n        },\n        {\n          \"description\": \"The maximum amount of time a worker may take to process\
  \ the activity task.\"\n        }\n      ]\n    },\n    \"taskList\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TaskList\"\n        },\n        {\n          \"description\": \"The task list in which the activity task has been scheduled.\"\n        }\n      ]\n    },\n    \"taskPriority\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TaskPriority\"\n        },\n        {\n          \"description\": \"<p> The priority to assign to the scheduled activity task. If set, this overrides any default priority value that was assigned when the activity type was registered.</p> <p>Valid values are integers that range from Java's <code>Integer.MIN_VALUE</code> (-2147483648) to <code>Integer.MAX_VALUE</code> (2147483647). Higher numbers indicate higher priority.</p> <p>For more information about setting task priority, see <a href=\\\"https://docs.aws.amazon.com/amazonswf/latest/developerguide/programming-priority.html\\\">Setting Task\
  \ Priority</a> in the <i>Amazon SWF Developer Guide</i>.</p>\"\n        }\n      ]\n    },\n    \"decisionTaskCompletedEventId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EventId\"\n        },\n        {\n          \"description\": \"The ID of the <code>DecisionTaskCompleted</code> event corresponding to the decision that resulted in the scheduling of this activity task. This information can be useful for diagnosing problems by tracing back the chain of events leading up to this event.\"\n        }\n      ]\n    },\n    \"heartbeatTimeout\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DurationInSecondsOptional\"\n        },\n        {\n          \"description\": \"The maximum time before which the worker processing this task must report progress by calling <a>RecordActivityTaskHeartbeat</a>. If the timeout is exceeded, the activity task is automatically timed out. If the worker subsequently attempts to record a heartbeat\
  \ or return a result, it is ignored.\"\n        }\n      ]\n    }\n  },\n  \"description\": \"Provides the details of the <code>ActivityTaskScheduled</code> event.\",\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"ActivityTaskScheduledEventAttributes\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-swf/refs/heads/main/json-schema/amazon-swf-activitytaskscheduledeventattributes-schema.json
tags:
- Automation
- AWS
- Task Coordination
- Workflow
title: ActivityTaskScheduledEventAttributes
---
