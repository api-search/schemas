---
description: The media stream that you want to add to the flow.
layout: schema
name: AddMediaStreamRequest
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
  name: MediaStreamId
  type: object
- description: ''
  name: MediaStreamName
  type: object
- description: ''
  name: MediaStreamType
  type: object
- description: ''
  name: VideoFormat
  type: object
provider_name: Amazon MediaConnect
provider_slug: amazon-mediaconnect
schema_file: json-schema/mediaconnect-api-add-media-stream-request-schema.json
slug: mediaconnect-api-add-media-stream-request
source_filename: mediaconnect-api-add-media-stream-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconnect/refs/heads/main/json-schema/mediaconnect-api-add-media-stream-request-schema.json\",\n  \"title\": \"AddMediaStreamRequest\",\n  \"description\": \"The media stream that you want to add to the flow.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Attributes\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MediaStreamAttributesRequest\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"attributes\"\n          },\n          \"description\": \"The attributes that you want to assign to the new media stream.\"\n        }\n      ]\n    },\n    \"ClockRate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integer\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"clockRate\"\n          },\n          \"description\": \"The\
  \ sample rate (in Hz) for the stream. If the media stream type is video or ancillary data, set this value to 90000. If the media stream type is audio, set this value to either 48000 or 96000.\"\n        }\n      ]\n    },\n    \"Description\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"description\"\n          },\n          \"description\": \"A description that can help you quickly identify what your media stream is used for.\"\n        }\n      ]\n    },\n    \"MediaStreamId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integer\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"mediaStreamId\"\n          },\n          \"description\": \"A unique identifier for the media stream.\"\n        }\n      ]\n    },\n    \"MediaStreamName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\
  \n        },\n        {\n          \"xml\": {\n            \"name\": \"mediaStreamName\"\n          },\n          \"description\": \"A name that helps you distinguish one media stream from another.\"\n        }\n      ]\n    },\n    \"MediaStreamType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MediaStreamType\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"mediaStreamType\"\n          },\n          \"description\": \"The type of media stream.\"\n        }\n      ]\n    },\n    \"VideoFormat\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"videoFormat\"\n          },\n          \"description\": \"The resolution of the video.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"MediaStreamType\",\n    \"MediaStreamId\",\n    \"MediaStreamName\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconnect/refs/heads/main/json-schema/mediaconnect-api-add-media-stream-request-schema.json
tags:
- Broadcasting
- Live Video
- Media
- Media Transport
title: AddMediaStreamRequest
---
