---
description: Provides the details of the <code>ActivityTaskFailed</code> event.
layout: schema
name: ActivityTaskFailedEventAttributes
properties_list:
- description: ''
  name: reason
  type: object
- description: ''
  name: details
  type: object
- description: ''
  name: scheduledEventId
  type: object
- description: ''
  name: startedEventId
  type: object
provider_name: Amazon Simple Workflow Service
provider_slug: amazon-swf
schema_file: json-schema/amazon-swf-activitytaskfailedeventattributes-schema.json
slug: amazon-swf-activitytaskfailedeventattributes
source_filename: amazon-swf-activitytaskfailedeventattributes-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"required\": [\n    \"scheduledEventId\",\n    \"startedEventId\"\n  ],\n  \"properties\": {\n    \"reason\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FailureReason\"\n        },\n        {\n          \"description\": \"The reason provided for the failure.\"\n        }\n      ]\n    },\n    \"details\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Data\"\n        },\n        {\n          \"description\": \"The details of the failure.\"\n        }\n      ]\n    },\n    \"scheduledEventId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EventId\"\n        },\n        {\n          \"description\": \"The ID of the <code>ActivityTaskScheduled</code> event that was recorded when this activity task was scheduled. This information can be useful for diagnosing problems by tracing back the chain of events leading up to this event.\"\n        }\n      ]\n \
  \   },\n    \"startedEventId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EventId\"\n        },\n        {\n          \"description\": \"The ID of the <code>ActivityTaskStarted</code> event recorded when this activity task was started. This information can be useful for diagnosing problems by tracing back the chain of events leading up to this event.\"\n        }\n      ]\n    }\n  },\n  \"description\": \"Provides the details of the <code>ActivityTaskFailed</code> event.\",\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"ActivityTaskFailedEventAttributes\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-swf/refs/heads/main/json-schema/amazon-swf-activitytaskfailedeventattributes-schema.json
tags:
- Automation
- AWS
- Task Coordination
- Workflow
title: ActivityTaskFailedEventAttributes
---
