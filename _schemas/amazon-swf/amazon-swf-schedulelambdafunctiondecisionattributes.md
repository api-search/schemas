---
description: Decision attributes specified in <code>scheduleLambdaFunctionDecisionAttributes</code> within the list of decisions <code>decisions</code> passed to <a>RespondDecisionTaskCompleted</a>.
layout: schema
name: ScheduleLambdaFunctionDecisionAttributes
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
provider_name: Amazon Simple Workflow Service
provider_slug: amazon-swf
schema_file: json-schema/amazon-swf-schedulelambdafunctiondecisionattributes-schema.json
slug: amazon-swf-schedulelambdafunctiondecisionattributes
source_filename: amazon-swf-schedulelambdafunctiondecisionattributes-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"required\": [\n    \"id\",\n    \"name\"\n  ],\n  \"properties\": {\n    \"id\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FunctionId\"\n        },\n        {\n          \"description\": \"A string that identifies the Lambda function execution in the event history.\"\n        }\n      ]\n    },\n    \"name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FunctionName\"\n        },\n        {\n          \"description\": \"The name, or ARN, of the Lambda function to schedule.\"\n        }\n      ]\n    },\n    \"control\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Data\"\n        },\n        {\n          \"description\": \"The data attached to the event that the decider can use in subsequent workflow tasks. This data isn't sent to the Lambda task.\"\n        }\n      ]\n    },\n    \"input\": {\n      \"allOf\": [\n        {\n          \"$ref\"\
  : \"#/components/schemas/FunctionInput\"\n        },\n        {\n          \"description\": \"The optional input data to be supplied to the Lambda function.\"\n        }\n      ]\n    },\n    \"startToCloseTimeout\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DurationInSecondsOptional\"\n        },\n        {\n          \"description\": \"<p>The timeout value, in seconds, after which the Lambda function is considered to be failed once it has started. This can be any integer from 1-900 (1s-15m).</p> <p>If no value is supplied, then a default value of 900s is assumed.</p>\"\n        }\n      ]\n    }\n  },\n  \"description\": \"Decision attributes specified in <code>scheduleLambdaFunctionDecisionAttributes</code> within the list of decisions <code>decisions</code> passed to <a>RespondDecisionTaskCompleted</a>.\",\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"ScheduleLambdaFunctionDecisionAttributes\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-swf/refs/heads/main/json-schema/amazon-swf-schedulelambdafunctiondecisionattributes-schema.json
tags:
- Automation
- AWS
- Task Coordination
- Workflow
title: ScheduleLambdaFunctionDecisionAttributes
---
