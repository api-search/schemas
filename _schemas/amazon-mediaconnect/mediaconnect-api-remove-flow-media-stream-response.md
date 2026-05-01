---
description: RemoveFlowMediaStreamResponse schema from AWS Elemental MediaConnect API
layout: schema
name: RemoveFlowMediaStreamResponse
properties_list:
- description: ''
  name: FlowArn
  type: object
- description: ''
  name: MediaStreamName
  type: object
provider_name: Amazon MediaConnect
provider_slug: amazon-mediaconnect
schema_file: json-schema/mediaconnect-api-remove-flow-media-stream-response-schema.json
slug: mediaconnect-api-remove-flow-media-stream-response
source_filename: mediaconnect-api-remove-flow-media-stream-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconnect/refs/heads/main/json-schema/mediaconnect-api-remove-flow-media-stream-response-schema.json\",\n  \"title\": \"RemoveFlowMediaStreamResponse\",\n  \"description\": \"RemoveFlowMediaStreamResponse schema from AWS Elemental MediaConnect API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"FlowArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"flowArn\"\n          },\n          \"description\": \"The Amazon Resource Name (ARN) of the flow.\"\n        }\n      ]\n    },\n    \"MediaStreamName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"mediaStreamName\"\n          },\n          \"description\": \"\
  The name of the media stream that was removed.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconnect/refs/heads/main/json-schema/mediaconnect-api-remove-flow-media-stream-response-schema.json
tags:
- Broadcasting
- Live Video
- Media
- Media Transport
title: RemoveFlowMediaStreamResponse
---
