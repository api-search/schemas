---
description: Error related to a specific channel, specified by its ARN.
layout: schema
name: BatchError
properties_list:
- description: ''
  name: arn
  type: object
- description: ''
  name: code
  type: object
- description: ''
  name: message
  type: object
provider_name: Amazon Interactive Video Service
provider_slug: amazon-interactive-video-service
schema_file: json-schema/ivs-batch-error-schema.json
slug: ivs-batch-error
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-interactive-video-service/refs/heads/main/json-schema/ivs-batch-error-schema.json\",\n  \"title\": \"BatchError\",\n  \"description\": \"Error related to a specific channel, specified by its ARN.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"arn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceArn\"\n        },\n        {\n          \"description\": \"Channel ARN.\"\n        }\n      ]\n    },\n    \"code\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/errorCode\"\n        },\n        {\n          \"description\": \"Error code.\"\n        }\n      ]\n    },\n    \"message\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/errorMessage\"\n        },\n        {\n          \"description\": \"Error message, determined by the application.\"\
  \n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-interactive-video-service/refs/heads/main/json-schema/ivs-batch-error-schema.json
tags:
- AWS
- Live Streaming
- Media
- Video
- Real-Time
title: BatchError
---
