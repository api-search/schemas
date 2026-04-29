---
description: Provides the details of the <code>ActivityTaskTimedOut</code> event.
layout: schema
name: ActivityTaskTimedOutEventAttributes
properties_list:
- description: ''
  name: timeoutType
  type: object
- description: ''
  name: scheduledEventId
  type: object
- description: ''
  name: startedEventId
  type: object
- description: ''
  name: details
  type: object
provider_name: Amazon Simple Workflow Service
provider_slug: amazon-swf
schema_file: json-schema/amazon-swf-activitytasktimedouteventattributes-schema.json
slug: amazon-swf-activitytasktimedouteventattributes
source_json: "{\n  \"type\": \"object\",\n  \"required\": [\n    \"timeoutType\",\n    \"scheduledEventId\",\n    \"startedEventId\"\n  ],\n  \"properties\": {\n    \"timeoutType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ActivityTaskTimeoutType\"\n        },\n        {\n          \"description\": \"The type of the timeout that caused this event.\"\n        }\n      ]\n    },\n    \"scheduledEventId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EventId\"\n        },\n        {\n          \"description\": \"The ID of the <code>ActivityTaskScheduled</code> event that was recorded when this activity task was scheduled. This information can be useful for diagnosing problems by tracing back the chain of events leading up to this event.\"\n        }\n      ]\n    },\n    \"startedEventId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EventId\"\n        },\n        {\n          \"description\"\
  : \"The ID of the <code>ActivityTaskStarted</code> event recorded when this activity task was started. This information can be useful for diagnosing problems by tracing back the chain of events leading up to this event.\"\n        }\n      ]\n    },\n    \"details\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LimitedData\"\n        },\n        {\n          \"description\": \"Contains the content of the <code>details</code> parameter for the last call made by the activity to <code>RecordActivityTaskHeartbeat</code>.\"\n        }\n      ]\n    }\n  },\n  \"description\": \"Provides the details of the <code>ActivityTaskTimedOut</code> event.\",\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"ActivityTaskTimedOutEventAttributes\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-swf/refs/heads/main/json-schema/amazon-swf-activitytasktimedouteventattributes-schema.json
tags:
- Automation
- AWS
- Task Coordination
- Workflow
title: ActivityTaskTimedOutEventAttributes
---
