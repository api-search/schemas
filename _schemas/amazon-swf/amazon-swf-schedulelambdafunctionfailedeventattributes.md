---
description: Provides the details of the <code>ScheduleLambdaFunctionFailed</code> event. It isn't set for other event types.
layout: schema
name: ScheduleLambdaFunctionFailedEventAttributes
properties_list:
- description: ''
  name: id
  type: object
- description: ''
  name: name
  type: object
- description: ''
  name: cause
  type: object
- description: ''
  name: decisionTaskCompletedEventId
  type: object
provider_name: Amazon Simple Workflow Service
provider_slug: amazon-swf
schema_file: json-schema/amazon-swf-schedulelambdafunctionfailedeventattributes-schema.json
slug: amazon-swf-schedulelambdafunctionfailedeventattributes
source_filename: amazon-swf-schedulelambdafunctionfailedeventattributes-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"required\": [\n    \"id\",\n    \"name\",\n    \"cause\",\n    \"decisionTaskCompletedEventId\"\n  ],\n  \"properties\": {\n    \"id\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FunctionId\"\n        },\n        {\n          \"description\": \"The ID provided in the <code>ScheduleLambdaFunction</code> decision that failed. \"\n        }\n      ]\n    },\n    \"name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FunctionName\"\n        },\n        {\n          \"description\": \"The name of the Lambda function.\"\n        }\n      ]\n    },\n    \"cause\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ScheduleLambdaFunctionFailedCause\"\n        },\n        {\n          \"description\": \"<p>The cause of the failure. To help diagnose issues, use this information to trace back the chain of events leading up to this event.</p> <note> <p>If <code>cause</code>\
  \ is set to <code>OPERATION_NOT_PERMITTED</code>, the decision failed because it lacked sufficient permissions. For details and example IAM policies, see <a href=\\\"https://docs.aws.amazon.com/amazonswf/latest/developerguide/swf-dev-iam.html\\\">Using IAM to Manage Access to Amazon SWF Workflows</a> in the <i>Amazon SWF Developer Guide</i>.</p> </note>\"\n        }\n      ]\n    },\n    \"decisionTaskCompletedEventId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EventId\"\n        },\n        {\n          \"description\": \"The ID of the <code>LambdaFunctionCompleted</code> event corresponding to the decision that resulted in scheduling this Lambda task. To help diagnose issues, use this information to trace back the chain of events leading up to this event.\"\n        }\n      ]\n    }\n  },\n  \"description\": \"Provides the details of the <code>ScheduleLambdaFunctionFailed</code> event. It isn't set for other event types.\",\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\"\
  ,\n  \"title\": \"ScheduleLambdaFunctionFailedEventAttributes\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-swf/refs/heads/main/json-schema/amazon-swf-schedulelambdafunctionfailedeventattributes-schema.json
tags:
- Automation
- Task Coordination
- Workflow
title: ScheduleLambdaFunctionFailedEventAttributes
---
