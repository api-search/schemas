---
description: Provides details about the <code>DecisionTaskScheduled</code> event.
layout: schema
name: DecisionTaskScheduledEventAttributes
properties_list:
- description: ''
  name: taskList
  type: object
- description: ''
  name: taskPriority
  type: object
- description: ''
  name: startToCloseTimeout
  type: object
provider_name: Amazon Simple Workflow Service
provider_slug: amazon-swf
schema_file: json-schema/amazon-swf-decisiontaskscheduledeventattributes-schema.json
slug: amazon-swf-decisiontaskscheduledeventattributes
source_filename: amazon-swf-decisiontaskscheduledeventattributes-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"required\": [\n    \"taskList\"\n  ],\n  \"properties\": {\n    \"taskList\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TaskList\"\n        },\n        {\n          \"description\": \"The name of the task list in which the decision task was scheduled.\"\n        }\n      ]\n    },\n    \"taskPriority\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TaskPriority\"\n        },\n        {\n          \"description\": \"<p> A task priority that, if set, specifies the priority for this decision task. Valid values are integers that range from Java's <code>Integer.MIN_VALUE</code> (-2147483648) to <code>Integer.MAX_VALUE</code> (2147483647). Higher numbers indicate higher priority.</p> <p>For more information about setting task priority, see <a href=\\\"https://docs.aws.amazon.com/amazonswf/latest/developerguide/programming-priority.html\\\">Setting Task Priority</a> in the <i>Amazon SWF\
  \ Developer Guide</i>.</p>\"\n        }\n      ]\n    },\n    \"startToCloseTimeout\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DurationInSecondsOptional\"\n        },\n        {\n          \"description\": \"<p>The maximum duration for this decision task. The task is considered timed out if it doesn't completed within this duration.</p> <p>The duration is specified in seconds, an integer greater than or equal to <code>0</code>. You can use <code>NONE</code> to specify unlimited duration.</p>\"\n        }\n      ]\n    }\n  },\n  \"description\": \"Provides details about the <code>DecisionTaskScheduled</code> event.\",\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"DecisionTaskScheduledEventAttributes\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-swf/refs/heads/main/json-schema/amazon-swf-decisiontaskscheduledeventattributes-schema.json
tags:
- Automation
- AWS
- Task Coordination
- Workflow
title: DecisionTaskScheduledEventAttributes
---
