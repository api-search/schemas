---
description: Provides the details of the <code>LambdaFunctionCompleted</code> event. It isn't set for other event types.
layout: schema
name: LambdaFunctionCompletedEventAttributes
properties_list:
- description: ''
  name: scheduledEventId
  type: object
- description: ''
  name: startedEventId
  type: object
- description: ''
  name: result
  type: object
provider_name: Amazon Simple Workflow Service
provider_slug: amazon-swf
schema_file: json-schema/amazon-swf-lambdafunctioncompletedeventattributes-schema.json
slug: amazon-swf-lambdafunctioncompletedeventattributes
source_json: "{\n  \"type\": \"object\",\n  \"required\": [\n    \"scheduledEventId\",\n    \"startedEventId\"\n  ],\n  \"properties\": {\n    \"scheduledEventId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EventId\"\n        },\n        {\n          \"description\": \"The ID of the <code>LambdaFunctionScheduled</code> event that was recorded when this Lambda task was scheduled. To help diagnose issues, use this information to trace back the chain of events leading up to this event.\"\n        }\n      ]\n    },\n    \"startedEventId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EventId\"\n        },\n        {\n          \"description\": \"The ID of the <code>LambdaFunctionStarted</code> event recorded when this activity task started. To help diagnose issues, use this information to trace back the chain of events leading up to this event.\"\n        }\n      ]\n    },\n    \"result\": {\n      \"allOf\": [\n        {\n\
  \          \"$ref\": \"#/components/schemas/Data\"\n        },\n        {\n          \"description\": \"The results of the Lambda task.\"\n        }\n      ]\n    }\n  },\n  \"description\": \"Provides the details of the <code>LambdaFunctionCompleted</code> event. It isn't set for other event types.\",\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"LambdaFunctionCompletedEventAttributes\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-swf/refs/heads/main/json-schema/amazon-swf-lambdafunctioncompletedeventattributes-schema.json
tags:
- Automation
- AWS
- Task Coordination
- Workflow
title: LambdaFunctionCompletedEventAttributes
---
