---
description: Provides details of the <code>LambdaFunctionTimedOut</code> event.
layout: schema
name: LambdaFunctionTimedOutEventAttributes
properties_list:
- description: ''
  name: scheduledEventId
  type: object
- description: ''
  name: startedEventId
  type: object
- description: ''
  name: timeoutType
  type: object
provider_name: Amazon Simple Workflow Service
provider_slug: amazon-swf
schema_file: json-schema/amazon-swf-lambdafunctiontimedouteventattributes-schema.json
slug: amazon-swf-lambdafunctiontimedouteventattributes
source_filename: amazon-swf-lambdafunctiontimedouteventattributes-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"required\": [\n    \"scheduledEventId\",\n    \"startedEventId\"\n  ],\n  \"properties\": {\n    \"scheduledEventId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EventId\"\n        },\n        {\n          \"description\": \"The ID of the <code>LambdaFunctionScheduled</code> event that was recorded when this activity task was scheduled. To help diagnose issues, use this information to trace back the chain of events leading up to this event.\"\n        }\n      ]\n    },\n    \"startedEventId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EventId\"\n        },\n        {\n          \"description\": \"The ID of the <code>ActivityTaskStarted</code> event that was recorded when this activity task started. To help diagnose issues, use this information to trace back the chain of events leading up to this event.\"\n        }\n      ]\n    },\n    \"timeoutType\": {\n      \"allOf\":\
  \ [\n        {\n          \"$ref\": \"#/components/schemas/LambdaFunctionTimeoutType\"\n        },\n        {\n          \"description\": \"The type of the timeout that caused this event.\"\n        }\n      ]\n    }\n  },\n  \"description\": \"Provides details of the <code>LambdaFunctionTimedOut</code> event.\",\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"LambdaFunctionTimedOutEventAttributes\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-swf/refs/heads/main/json-schema/amazon-swf-lambdafunctiontimedouteventattributes-schema.json
tags:
- Automation
- Task Coordination
- Workflow
title: LambdaFunctionTimedOutEventAttributes
---
