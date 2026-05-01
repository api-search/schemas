---
description: Provides the details of the <code>LambdaFunctionScheduled</code> event. It isn't set for other event types.
layout: schema
name: LambdaFunctionScheduledEventAttributes
properties_list:
- description: ''
  name: id
  type: object
- description: ''
  name: name
  type: object
- description: ''
  name: control
  type: object
- description: ''
  name: input
  type: object
- description: ''
  name: startToCloseTimeout
  type: object
- description: ''
  name: decisionTaskCompletedEventId
  type: object
provider_name: Amazon Simple Workflow Service
provider_slug: amazon-swf
schema_file: json-schema/amazon-swf-lambdafunctionscheduledeventattributes-schema.json
slug: amazon-swf-lambdafunctionscheduledeventattributes
source_filename: amazon-swf-lambdafunctionscheduledeventattributes-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"required\": [\n    \"id\",\n    \"name\",\n    \"decisionTaskCompletedEventId\"\n  ],\n  \"properties\": {\n    \"id\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FunctionId\"\n        },\n        {\n          \"description\": \"The unique ID of the Lambda task.\"\n        }\n      ]\n    },\n    \"name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FunctionName\"\n        },\n        {\n          \"description\": \"The name of the Lambda function.\"\n        }\n      ]\n    },\n    \"control\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Data\"\n        },\n        {\n          \"description\": \"Data attached to the event that the decider can use in subsequent workflow tasks. This data isn't sent to the Lambda task.\"\n        }\n      ]\n    },\n    \"input\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FunctionInput\"\
  \n        },\n        {\n          \"description\": \"The input provided to the Lambda task.\"\n        }\n      ]\n    },\n    \"startToCloseTimeout\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DurationInSecondsOptional\"\n        },\n        {\n          \"description\": \"The maximum amount of time a worker can take to process the Lambda task.\"\n        }\n      ]\n    },\n    \"decisionTaskCompletedEventId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EventId\"\n        },\n        {\n          \"description\": \"The ID of the <code>LambdaFunctionCompleted</code> event corresponding to the decision that resulted in scheduling this activity task. To help diagnose issues, use this information to trace back the chain of events leading up to this event.\"\n        }\n      ]\n    }\n  },\n  \"description\": \"Provides the details of the <code>LambdaFunctionScheduled</code> event. It isn't set for other event types.\"\
  ,\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"LambdaFunctionScheduledEventAttributes\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-swf/refs/heads/main/json-schema/amazon-swf-lambdafunctionscheduledeventattributes-schema.json
tags:
- Automation
- Task Coordination
- Workflow
title: LambdaFunctionScheduledEventAttributes
---
