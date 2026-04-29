---
description: The fields that you want to update in the media stream.
layout: schema
name: UpdateFlowMediaStreamRequest
properties_list:
- description: ''
  name: Attributes
  type: object
- description: ''
  name: ClockRate
  type: object
- description: ''
  name: Description
  type: object
- description: ''
  name: MediaStreamType
  type: object
- description: ''
  name: VideoFormat
  type: object
provider_name: Amazon MediaConnect
provider_slug: amazon-mediaconnect
schema_file: json-schema/mediaconnect-api-update-flow-media-stream-request-schema.json
slug: mediaconnect-api-update-flow-media-stream-request
source_filename: mediaconnect-api-update-flow-media-stream-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconnect/refs/heads/main/json-schema/mediaconnect-api-update-flow-media-stream-request-schema.json\",\n  \"title\": \"UpdateFlowMediaStreamRequest\",\n  \"description\": \"The fields that you want to update in the media stream.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Attributes\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MediaStreamAttributesRequest\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"attributes\"\n          },\n          \"description\": \"The attributes that you want to assign to the media stream.\"\n        }\n      ]\n    },\n    \"ClockRate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integer\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"clockRate\"\n          },\n          \"description\"\
  : \"The sample rate (in Hz) for the stream. If the media stream type is video or ancillary data, set this value to 90000. If the media stream type is audio, set this value to either 48000 or 96000.\"\n        }\n      ]\n    },\n    \"Description\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"description\"\n          },\n          \"description\": \"Description\"\n        }\n      ]\n    },\n    \"MediaStreamType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MediaStreamType\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"mediaStreamType\"\n          },\n          \"description\": \"The type of media stream.\"\n        }\n      ]\n    },\n    \"VideoFormat\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"videoFormat\"\
  \n          },\n          \"description\": \"The resolution of the video.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconnect/refs/heads/main/json-schema/mediaconnect-api-update-flow-media-stream-request-schema.json
tags:
- AWS
- Broadcasting
- Live Video
- Media
- Media Transport
title: UpdateFlowMediaStreamRequest
---
