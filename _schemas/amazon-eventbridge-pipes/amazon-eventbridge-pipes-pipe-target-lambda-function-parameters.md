---
description: The parameters for using a Lambda function as a target.
layout: schema
name: PipeTargetLambdaFunctionParameters
properties_list:
- description: ''
  name: InvocationType
  type: object
provider_name: Amazon EventBridge Pipes
provider_slug: amazon-eventbridge-pipes
schema_file: json-schema/amazon-eventbridge-pipes-pipe-target-lambda-function-parameters-schema.json
slug: amazon-eventbridge-pipes-pipe-target-lambda-function-parameters
source_filename: amazon-eventbridge-pipes-pipe-target-lambda-function-parameters-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-eventbridge-pipes/refs/heads/main/json-schema/amazon-eventbridge-pipes-pipe-target-lambda-function-parameters-schema.json\",\n  \"title\": \"PipeTargetLambdaFunctionParameters\",\n  \"description\": \"The parameters for using a Lambda function as a target.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"InvocationType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PipeTargetInvocationType\"\n        },\n        {\n          \"description\": \"<p>Choose from the following options.</p> <ul> <li> <p> <code>RequestResponse</code> (default) - Invoke the function synchronously. Keep the connection open until the function returns a response or times out. The API response includes the function response and additional data.</p> </li> <li> <p> <code>Event</code> - Invoke the function asynchronously. Send events\
  \ that fail multiple times to the function's dead-letter queue (if it's configured). The API response only includes a status code.</p> </li> <li> <p> <code>DryRun</code> - Validate parameter values and verify that the user or role has permission to invoke the function.</p> </li> </ul>\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-eventbridge-pipes/refs/heads/main/json-schema/amazon-eventbridge-pipes-pipe-target-lambda-function-parameters-schema.json
tags:
- Amazon Web Services
- Event-Driven
- Integration
- Messaging
- Serverless
title: PipeTargetLambdaFunctionParameters
---
