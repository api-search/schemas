---
description: AddFlowMediaStreamsResponse schema from AWS Elemental MediaConnect API
layout: schema
name: AddFlowMediaStreamsResponse
properties_list:
- description: ''
  name: FlowArn
  type: object
- description: ''
  name: MediaStreams
  type: object
provider_name: Amazon MediaConnect
provider_slug: amazon-mediaconnect
schema_file: json-schema/mediaconnect-api-add-flow-media-streams-response-schema.json
slug: mediaconnect-api-add-flow-media-streams-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconnect/refs/heads/main/json-schema/mediaconnect-api-add-flow-media-streams-response-schema.json\",\n  \"title\": \"AddFlowMediaStreamsResponse\",\n  \"description\": \"AddFlowMediaStreamsResponse schema from AWS Elemental MediaConnect API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"FlowArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"flowArn\"\n          },\n          \"description\": \"The ARN of the flow that you added media streams to.\"\n        }\n      ]\n    },\n    \"MediaStreams\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__listOfMediaStream\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"mediaStreams\"\n          },\n          \"description\"\
  : \"The media streams that you added to the flow.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconnect/refs/heads/main/json-schema/mediaconnect-api-add-flow-media-streams-response-schema.json
tags:
- AWS
- Broadcasting
- Live Video
- Media
- Media Transport
title: AddFlowMediaStreamsResponse
---
