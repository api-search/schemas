---
description: DeleteStreamKeyRequest schema
layout: schema
name: DeleteStreamKeyRequest
properties_list:
- description: ''
  name: arn
  type: object
provider_name: Amazon Interactive Video Service
provider_slug: amazon-interactive-video-service
schema_file: json-schema/ivs-delete-stream-key-request-schema.json
slug: ivs-delete-stream-key-request
source_filename: ivs-delete-stream-key-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-interactive-video-service/refs/heads/main/json-schema/ivs-delete-stream-key-request-schema.json\",\n  \"title\": \"DeleteStreamKeyRequest\",\n  \"description\": \"DeleteStreamKeyRequest schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"arn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StreamKeyArn\"\n        },\n        {\n          \"description\": \"ARN of the stream key to be deleted.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"arn\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-interactive-video-service/refs/heads/main/json-schema/ivs-delete-stream-key-request-schema.json
tags:
- AWS
- Live Streaming
- Media
- Video
- Real-Time
title: DeleteStreamKeyRequest
---
