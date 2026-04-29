---
description: An object that represents a pipe. Amazon EventBridgePipes connect event sources to targets and reduces the need for specialized knowledge and integration code.
layout: schema
name: Pipe
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
  name: Enrichment
  type: object
- description: ''
  name: LastModifiedTime
  type: object
- description: ''
  name: Name
  type: object
- description: ''
  name: Source
  type: object
- description: ''
  name: StateReason
  type: object
- description: ''
  name: Target
  type: object
provider_name: Amazon EventBridge Pipes
provider_slug: amazon-eventbridge-pipes
schema_file: json-schema/amazon-eventbridge-pipes-pipe-schema.json
slug: amazon-eventbridge-pipes-pipe
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-eventbridge-pipes/refs/heads/main/json-schema/amazon-eventbridge-pipes-pipe-schema.json\",\n  \"title\": \"Pipe\",\n  \"description\": \"An object that represents a pipe. Amazon EventBridgePipes connect event sources to targets and reduces the need for specialized knowledge and integration code.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Arn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PipeArn\"\n        },\n        {\n          \"description\": \"The ARN of the pipe.\"\n        }\n      ]\n    },\n    \"CreationTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The time the pipe was created.\"\n        }\n      ]\n    },\n    \"CurrentState\": {\n      \"allOf\": [\n        {\n          \"$ref\"\
  : \"#/components/schemas/PipeState\"\n        },\n        {\n          \"description\": \"The state the pipe is in.\"\n        }\n      ]\n    },\n    \"DesiredState\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RequestedPipeState\"\n        },\n        {\n          \"description\": \"The state the pipe should be in.\"\n        }\n      ]\n    },\n    \"Enrichment\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/OptionalArn\"\n        },\n        {\n          \"description\": \"The ARN of the enrichment resource.\"\n        }\n      ]\n    },\n    \"LastModifiedTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"When the pipe was last updated, in <a href=\\\"https://www.w3.org/TR/NOTE-datetime\\\">ISO-8601 format</a> (YYYY-MM-DDThh:mm:ss.sTZD).\"\n        }\n      ]\n    },\n    \"Name\": {\n      \"allOf\": [\n        {\n  \
  \        \"$ref\": \"#/components/schemas/PipeName\"\n        },\n        {\n          \"description\": \"The name of the pipe.\"\n        }\n      ]\n    },\n    \"Source\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ArnOrUrl\"\n        },\n        {\n          \"description\": \"The ARN of the source resource.\"\n        }\n      ]\n    },\n    \"StateReason\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PipeStateReason\"\n        },\n        {\n          \"description\": \"The reason the pipe is in its current state.\"\n        }\n      ]\n    },\n    \"Target\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Arn\"\n        },\n        {\n          \"description\": \"The ARN of the target resource.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-eventbridge-pipes/refs/heads/main/json-schema/amazon-eventbridge-pipes-pipe-schema.json
tags:
- Amazon Web Services
- AWS
- Event-Driven
- Integration
- Messaging
- Serverless
title: Pipe
---
