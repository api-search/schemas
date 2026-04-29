---
description: Provides the details of the <code>LambdaFunctionStarted</code> event. It isn't set for other event types.
layout: schema
name: LambdaFunctionStartedEventAttributes
properties_list:
- description: ''
  name: scheduledEventId
  type: object
provider_name: Amazon Simple Workflow Service
provider_slug: amazon-swf
schema_file: json-schema/amazon-swf-lambdafunctionstartedeventattributes-schema.json
slug: amazon-swf-lambdafunctionstartedeventattributes
source_filename: amazon-swf-lambdafunctionstartedeventattributes-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"required\": [\n    \"scheduledEventId\"\n  ],\n  \"properties\": {\n    \"scheduledEventId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EventId\"\n        },\n        {\n          \"description\": \"The ID of the <code>LambdaFunctionScheduled</code> event that was recorded when this activity task was scheduled. To help diagnose issues, use this information to trace back the chain of events leading up to this event.\"\n        }\n      ]\n    }\n  },\n  \"description\": \"Provides the details of the <code>LambdaFunctionStarted</code> event. It isn't set for other event types.\",\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"LambdaFunctionStartedEventAttributes\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-swf/refs/heads/main/json-schema/amazon-swf-lambdafunctionstartedeventattributes-schema.json
tags:
- Automation
- AWS
- Task Coordination
- Workflow
title: LambdaFunctionStartedEventAttributes
---
