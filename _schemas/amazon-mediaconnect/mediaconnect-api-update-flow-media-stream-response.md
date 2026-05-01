---
description: UpdateFlowMediaStreamResponse schema from AWS Elemental MediaConnect API
layout: schema
name: UpdateFlowMediaStreamResponse
properties_list:
- description: ''
  name: FlowArn
  type: object
- description: ''
  name: MediaStream
  type: object
provider_name: Amazon MediaConnect
provider_slug: amazon-mediaconnect
schema_file: json-schema/mediaconnect-api-update-flow-media-stream-response-schema.json
slug: mediaconnect-api-update-flow-media-stream-response
source_filename: mediaconnect-api-update-flow-media-stream-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconnect/refs/heads/main/json-schema/mediaconnect-api-update-flow-media-stream-response-schema.json\",\n  \"title\": \"UpdateFlowMediaStreamResponse\",\n  \"description\": \"UpdateFlowMediaStreamResponse schema from AWS Elemental MediaConnect API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"FlowArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"flowArn\"\n          },\n          \"description\": \"The ARN of the flow that is associated with the media stream that you updated.\"\n        }\n      ]\n    },\n    \"MediaStream\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MediaStream\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"mediaStream\"\n          },\n\
  \          \"description\": \"The media stream that you updated.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconnect/refs/heads/main/json-schema/mediaconnect-api-update-flow-media-stream-response-schema.json
tags:
- Broadcasting
- Live Video
- Media
- Media Transport
title: UpdateFlowMediaStreamResponse
---
