---
description: Provides the details of the <code>TimerCanceled</code> event.
layout: schema
name: TimerCanceledEventAttributes
properties_list:
- description: ''
  name: timerId
  type: object
- description: ''
  name: startedEventId
  type: object
- description: ''
  name: decisionTaskCompletedEventId
  type: object
provider_name: Amazon Simple Workflow Service
provider_slug: amazon-swf
schema_file: json-schema/amazon-swf-timercanceledeventattributes-schema.json
slug: amazon-swf-timercanceledeventattributes
source_json: "{\n  \"type\": \"object\",\n  \"required\": [\n    \"timerId\",\n    \"startedEventId\",\n    \"decisionTaskCompletedEventId\"\n  ],\n  \"properties\": {\n    \"timerId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TimerId\"\n        },\n        {\n          \"description\": \"The unique ID of the timer that was canceled.\"\n        }\n      ]\n    },\n    \"startedEventId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EventId\"\n        },\n        {\n          \"description\": \"The ID of the <code>TimerStarted</code> event that was recorded when this timer was started. This information can be useful for diagnosing problems by tracing back the chain of events leading up to this event.\"\n        }\n      ]\n    },\n    \"decisionTaskCompletedEventId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EventId\"\n        },\n        {\n          \"description\": \"The ID of the <code>DecisionTaskCompleted</code>\
  \ event corresponding to the decision task that resulted in the <code>CancelTimer</code> decision to cancel this timer. This information can be useful for diagnosing problems by tracing back the chain of events leading up to this event.\"\n        }\n      ]\n    }\n  },\n  \"description\": \" Provides the details of the <code>TimerCanceled</code> event. \",\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"TimerCanceledEventAttributes\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-swf/refs/heads/main/json-schema/amazon-swf-timercanceledeventattributes-schema.json
tags:
- Automation
- AWS
- Task Coordination
- Workflow
title: TimerCanceledEventAttributes
---
