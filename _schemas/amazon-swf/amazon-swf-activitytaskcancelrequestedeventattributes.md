---
description: Provides the details of the <code>ActivityTaskCancelRequested</code> event.
layout: schema
name: ActivityTaskCancelRequestedEventAttributes
properties_list:
- description: ''
  name: decisionTaskCompletedEventId
  type: object
- description: ''
  name: activityId
  type: object
provider_name: Amazon Simple Workflow Service
provider_slug: amazon-swf
schema_file: json-schema/amazon-swf-activitytaskcancelrequestedeventattributes-schema.json
slug: amazon-swf-activitytaskcancelrequestedeventattributes
source_filename: amazon-swf-activitytaskcancelrequestedeventattributes-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"required\": [\n    \"decisionTaskCompletedEventId\",\n    \"activityId\"\n  ],\n  \"properties\": {\n    \"decisionTaskCompletedEventId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EventId\"\n        },\n        {\n          \"description\": \"The ID of the <code>DecisionTaskCompleted</code> event corresponding to the decision task that resulted in the <code>RequestCancelActivityTask</code> decision for this cancellation request. This information can be useful for diagnosing problems by tracing back the chain of events leading up to this event.\"\n        }\n      ]\n    },\n    \"activityId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ActivityId\"\n        },\n        {\n          \"description\": \"The unique ID of the task.\"\n        }\n      ]\n    }\n  },\n  \"description\": \"Provides the details of the <code>ActivityTaskCancelRequested</code> event.\",\n  \"$schema\"\
  : \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"ActivityTaskCancelRequestedEventAttributes\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-swf/refs/heads/main/json-schema/amazon-swf-activitytaskcancelrequestedeventattributes-schema.json
tags:
- Automation
- Task Coordination
- Workflow
title: ActivityTaskCancelRequestedEventAttributes
---
