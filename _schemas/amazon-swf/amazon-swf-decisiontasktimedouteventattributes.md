---
description: Provides the details of the <code>DecisionTaskTimedOut</code> event.
layout: schema
name: DecisionTaskTimedOutEventAttributes
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
provider_name: Amazon Simple Workflow Service
provider_slug: amazon-swf
schema_file: json-schema/amazon-swf-decisiontasktimedouteventattributes-schema.json
slug: amazon-swf-decisiontasktimedouteventattributes
source_filename: amazon-swf-decisiontasktimedouteventattributes-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"required\": [\n    \"timeoutType\",\n    \"scheduledEventId\",\n    \"startedEventId\"\n  ],\n  \"properties\": {\n    \"timeoutType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DecisionTaskTimeoutType\"\n        },\n        {\n          \"description\": \"The type of timeout that expired before the decision task could be completed.\"\n        }\n      ]\n    },\n    \"scheduledEventId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EventId\"\n        },\n        {\n          \"description\": \"The ID of the <code>DecisionTaskScheduled</code> event that was recorded when this decision task was scheduled. This information can be useful for diagnosing problems by tracing back the chain of events leading up to this event.\"\n        }\n      ]\n    },\n    \"startedEventId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EventId\"\n        },\n    \
  \    {\n          \"description\": \"The ID of the <code>DecisionTaskStarted</code> event recorded when this decision task was started. This information can be useful for diagnosing problems by tracing back the chain of events leading up to this event.\"\n        }\n      ]\n    }\n  },\n  \"description\": \"Provides the details of the <code>DecisionTaskTimedOut</code> event.\",\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"DecisionTaskTimedOutEventAttributes\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-swf/refs/heads/main/json-schema/amazon-swf-decisiontasktimedouteventattributes-schema.json
tags:
- Automation
- AWS
- Task Coordination
- Workflow
title: DecisionTaskTimedOutEventAttributes
---
