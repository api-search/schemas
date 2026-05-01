---
description: Provides the details of the <code>StartLambdaFunctionFailed</code> event. It isn't set for other event types.
layout: schema
name: StartLambdaFunctionFailedEventAttributes
properties_list:
- description: ''
  name: scheduledEventId
  type: object
- description: ''
  name: cause
  type: object
- description: ''
  name: message
  type: object
provider_name: Amazon Simple Workflow Service
provider_slug: amazon-swf
schema_file: json-schema/amazon-swf-startlambdafunctionfailedeventattributes-schema.json
slug: amazon-swf-startlambdafunctionfailedeventattributes
source_filename: amazon-swf-startlambdafunctionfailedeventattributes-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"scheduledEventId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EventId\"\n        },\n        {\n          \"description\": \"The ID of the <code>ActivityTaskScheduled</code> event that was recorded when this activity task was scheduled. To help diagnose issues, use this information to trace back the chain of events leading up to this event.\"\n        }\n      ]\n    },\n    \"cause\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StartLambdaFunctionFailedCause\"\n        },\n        {\n          \"description\": \"<p>The cause of the failure. To help diagnose issues, use this information to trace back the chain of events leading up to this event.</p> <note> <p>If <code>cause</code> is set to <code>OPERATION_NOT_PERMITTED</code>, the decision failed because the IAM role attached to the execution lacked sufficient permissions. For details and example IAM policies,\
  \ see <a href=\\\"https://docs.aws.amazon.com/amazonswf/latest/developerguide/lambda-task.html\\\">Lambda Tasks</a> in the <i>Amazon SWF Developer Guide</i>.</p> </note>\"\n        }\n      ]\n    },\n    \"message\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CauseMessage\"\n        },\n        {\n          \"description\": \"A description that can help diagnose the cause of the fault.\"\n        }\n      ]\n    }\n  },\n  \"description\": \"Provides the details of the <code>StartLambdaFunctionFailed</code> event. It isn't set for other event types.\",\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"StartLambdaFunctionFailedEventAttributes\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-swf/refs/heads/main/json-schema/amazon-swf-startlambdafunctionfailedeventattributes-schema.json
tags:
- Automation
- Task Coordination
- Workflow
title: StartLambdaFunctionFailedEventAttributes
---
