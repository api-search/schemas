---
description: A request to add media streams to the flow.
layout: schema
name: AddFlowMediaStreamsRequest
properties_list:
- description: ''
  name: MediaStreams
  type: object
provider_name: Amazon MediaConnect
provider_slug: amazon-mediaconnect
schema_file: json-schema/mediaconnect-api-add-flow-media-streams-request-schema.json
slug: mediaconnect-api-add-flow-media-streams-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconnect/refs/heads/main/json-schema/mediaconnect-api-add-flow-media-streams-request-schema.json\",\n  \"title\": \"AddFlowMediaStreamsRequest\",\n  \"description\": \"A request to add media streams to the flow.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"MediaStreams\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__listOfAddMediaStreamRequest\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"mediaStreams\"\n          },\n          \"description\": \"The media streams that you want to add to the flow.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"MediaStreams\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconnect/refs/heads/main/json-schema/mediaconnect-api-add-flow-media-streams-request-schema.json
tags:
- AWS
- Broadcasting
- Live Video
- Media
- Media Transport
title: AddFlowMediaStreamsRequest
---
