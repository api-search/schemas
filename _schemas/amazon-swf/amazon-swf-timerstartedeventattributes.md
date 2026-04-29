---
description: Provides the details of the <code>TimerStarted</code> event.
layout: schema
name: TimerStartedEventAttributes
properties_list:
- description: ''
  name: timerId
  type: object
- description: ''
  name: control
  type: object
- description: ''
  name: startToFireTimeout
  type: object
- description: ''
  name: decisionTaskCompletedEventId
  type: object
provider_name: Amazon Simple Workflow Service
provider_slug: amazon-swf
schema_file: json-schema/amazon-swf-timerstartedeventattributes-schema.json
slug: amazon-swf-timerstartedeventattributes
source_json: "{\n  \"type\": \"object\",\n  \"required\": [\n    \"timerId\",\n    \"startToFireTimeout\",\n    \"decisionTaskCompletedEventId\"\n  ],\n  \"properties\": {\n    \"timerId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TimerId\"\n        },\n        {\n          \"description\": \"The unique ID of the timer that was started.\"\n        }\n      ]\n    },\n    \"control\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Data\"\n        },\n        {\n          \"description\": \"Data attached to the event that can be used by the decider in subsequent workflow tasks.\"\n        }\n      ]\n    },\n    \"startToFireTimeout\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DurationInSeconds\"\n        },\n        {\n          \"description\": \"<p>The duration of time after which the timer fires.</p> <p>The duration is specified in seconds, an integer greater than or equal to <code>0</code>.</p>\"\
  \n        }\n      ]\n    },\n    \"decisionTaskCompletedEventId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EventId\"\n        },\n        {\n          \"description\": \"The ID of the <code>DecisionTaskCompleted</code> event corresponding to the decision task that resulted in the <code>StartTimer</code> decision for this activity task. This information can be useful for diagnosing problems by tracing back the chain of events leading up to this event.\"\n        }\n      ]\n    }\n  },\n  \"description\": \"Provides the details of the <code>TimerStarted</code> event.\",\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"TimerStartedEventAttributes\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-swf/refs/heads/main/json-schema/amazon-swf-timerstartedeventattributes-schema.json
tags:
- Automation
- AWS
- Task Coordination
- Workflow
title: TimerStartedEventAttributes
---
