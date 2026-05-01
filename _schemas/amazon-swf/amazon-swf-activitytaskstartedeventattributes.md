---
description: Provides the details of the <code>ActivityTaskStarted</code> event.
layout: schema
name: ActivityTaskStartedEventAttributes
properties_list:
- description: ''
  name: identity
  type: object
- description: ''
  name: scheduledEventId
  type: object
provider_name: Amazon Simple Workflow Service
provider_slug: amazon-swf
schema_file: json-schema/amazon-swf-activitytaskstartedeventattributes-schema.json
slug: amazon-swf-activitytaskstartedeventattributes
source_filename: amazon-swf-activitytaskstartedeventattributes-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"required\": [\n    \"scheduledEventId\"\n  ],\n  \"properties\": {\n    \"identity\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Identity\"\n        },\n        {\n          \"description\": \"Identity of the worker that was assigned this task. This aids diagnostics when problems arise. The form of this identity is user defined.\"\n        }\n      ]\n    },\n    \"scheduledEventId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EventId\"\n        },\n        {\n          \"description\": \"The ID of the <code>ActivityTaskScheduled</code> event that was recorded when this activity task was scheduled. This information can be useful for diagnosing problems by tracing back the chain of events leading up to this event.\"\n        }\n      ]\n    }\n  },\n  \"description\": \"Provides the details of the <code>ActivityTaskStarted</code> event.\",\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\"\
  ,\n  \"title\": \"ActivityTaskStartedEventAttributes\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-swf/refs/heads/main/json-schema/amazon-swf-activitytaskstartedeventattributes-schema.json
tags:
- Automation
- Task Coordination
- Workflow
title: ActivityTaskStartedEventAttributes
---
