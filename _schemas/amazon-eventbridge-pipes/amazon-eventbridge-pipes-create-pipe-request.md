---
description: CreatePipeRequest schema from Amazon EventBridge Pipes
layout: schema
name: CreatePipeRequest
properties_list:
- description: ''
  name: Description
  type: object
- description: ''
  name: DesiredState
  type: object
- description: ''
  name: Enrichment
  type: object
- description: ''
  name: EnrichmentParameters
  type: object
- description: ''
  name: RoleArn
  type: object
- description: ''
  name: Source
  type: object
- description: ''
  name: SourceParameters
  type: object
- description: ''
  name: Tags
  type: object
- description: ''
  name: Target
  type: object
- description: ''
  name: TargetParameters
  type: object
provider_name: Amazon EventBridge Pipes
provider_slug: amazon-eventbridge-pipes
schema_file: json-schema/amazon-eventbridge-pipes-create-pipe-request-schema.json
slug: amazon-eventbridge-pipes-create-pipe-request
source_filename: amazon-eventbridge-pipes-create-pipe-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-eventbridge-pipes/refs/heads/main/json-schema/amazon-eventbridge-pipes-create-pipe-request-schema.json\",\n  \"title\": \"CreatePipeRequest\",\n  \"description\": \"CreatePipeRequest schema from Amazon EventBridge Pipes\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Description\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PipeDescription\"\n        },\n        {\n          \"description\": \"A description of the pipe.\"\n        }\n      ]\n    },\n    \"DesiredState\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RequestedPipeState\"\n        },\n        {\n          \"description\": \"The state the pipe should be in.\"\n        }\n      ]\n    },\n    \"Enrichment\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/OptionalArn\"\n   \
  \     },\n        {\n          \"description\": \"The ARN of the enrichment resource.\"\n        }\n      ]\n    },\n    \"EnrichmentParameters\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PipeEnrichmentParameters\"\n        },\n        {\n          \"description\": \"The parameters required to set up enrichment on your pipe.\"\n        }\n      ]\n    },\n    \"RoleArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RoleArn\"\n        },\n        {\n          \"description\": \"The ARN of the role that allows the pipe to send data to the target.\"\n        }\n      ]\n    },\n    \"Source\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ArnOrUrl\"\n        },\n        {\n          \"description\": \"The ARN of the source resource.\"\n        }\n      ]\n    },\n    \"SourceParameters\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PipeSourceParameters\"\n \
  \       },\n        {\n          \"description\": \"The parameters required to set up a source for your pipe.\"\n        }\n      ]\n    },\n    \"Tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TagMap\"\n        },\n        {\n          \"description\": \"The list of key-value pairs to associate with the pipe.\"\n        }\n      ]\n    },\n    \"Target\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Arn\"\n        },\n        {\n          \"description\": \"The ARN of the target resource.\"\n        }\n      ]\n    },\n    \"TargetParameters\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PipeTargetParameters\"\n        },\n        {\n          \"description\": \"The parameters required to set up a target for your pipe.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"RoleArn\",\n    \"Source\",\n    \"Target\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-eventbridge-pipes/refs/heads/main/json-schema/amazon-eventbridge-pipes-create-pipe-request-schema.json
tags:
- Amazon Web Services
- Event-Driven
- Integration
- Messaging
- Serverless
title: CreatePipeRequest
---
