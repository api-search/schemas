---
description: DeletePipeResponse schema from Amazon EventBridge Pipes
layout: schema
name: DeletePipeResponse
properties_list:
- description: ''
  name: Arn
  type: object
- description: ''
  name: CreationTime
  type: object
- description: ''
  name: CurrentState
  type: object
- description: ''
  name: DesiredState
  type: object
- description: ''
  name: LastModifiedTime
  type: object
- description: ''
  name: Name
  type: object
provider_name: Amazon EventBridge Pipes
provider_slug: amazon-eventbridge-pipes
schema_file: json-schema/amazon-eventbridge-pipes-delete-pipe-response-schema.json
slug: amazon-eventbridge-pipes-delete-pipe-response
source_filename: amazon-eventbridge-pipes-delete-pipe-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-eventbridge-pipes/refs/heads/main/json-schema/amazon-eventbridge-pipes-delete-pipe-response-schema.json\",\n  \"title\": \"DeletePipeResponse\",\n  \"description\": \"DeletePipeResponse schema from Amazon EventBridge Pipes\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Arn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PipeArn\"\n        },\n        {\n          \"description\": \"The ARN of the pipe.\"\n        }\n      ]\n    },\n    \"CreationTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The time the pipe was created.\"\n        }\n      ]\n    },\n    \"CurrentState\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PipeState\"\n        },\n        {\n          \"\
  description\": \"The state the pipe is in.\"\n        }\n      ]\n    },\n    \"DesiredState\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RequestedPipeStateDescribeResponse\"\n        },\n        {\n          \"description\": \"The state the pipe should be in.\"\n        }\n      ]\n    },\n    \"LastModifiedTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"When the pipe was last updated, in <a href=\\\"https://www.w3.org/TR/NOTE-datetime\\\">ISO-8601 format</a> (YYYY-MM-DDThh:mm:ss.sTZD).\"\n        }\n      ]\n    },\n    \"Name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PipeName\"\n        },\n        {\n          \"description\": \"The name of the pipe.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-eventbridge-pipes/refs/heads/main/json-schema/amazon-eventbridge-pipes-delete-pipe-response-schema.json
tags:
- Amazon Web Services
- Event-Driven
- Integration
- Messaging
- Serverless
title: DeletePipeResponse
---
