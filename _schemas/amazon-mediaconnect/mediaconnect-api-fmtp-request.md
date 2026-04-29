---
description: The settings that you want to use to define the media stream.
layout: schema
name: FmtpRequest
properties_list:
- description: ''
  name: ChannelOrder
  type: object
- description: ''
  name: Colorimetry
  type: object
- description: ''
  name: ExactFramerate
  type: object
- description: ''
  name: Par
  type: object
- description: ''
  name: Range
  type: object
- description: ''
  name: ScanMode
  type: object
- description: ''
  name: Tcs
  type: object
provider_name: Amazon MediaConnect
provider_slug: amazon-mediaconnect
schema_file: json-schema/mediaconnect-api-fmtp-request-schema.json
slug: mediaconnect-api-fmtp-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconnect/refs/heads/main/json-schema/mediaconnect-api-fmtp-request-schema.json\",\n  \"title\": \"FmtpRequest\",\n  \"description\": \"The settings that you want to use to define the media stream.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ChannelOrder\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"channelOrder\"\n          },\n          \"description\": \"The format of the audio channel.\"\n        }\n      ]\n    },\n    \"Colorimetry\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Colorimetry\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"colorimetry\"\n          },\n          \"description\": \"The format that is used for the representation of color.\"\
  \n        }\n      ]\n    },\n    \"ExactFramerate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"exactFramerate\"\n          },\n          \"description\": \"The frame rate for the video stream, in frames/second. For example: 60000/1001. If you specify a whole number, MediaConnect uses a ratio of N/1. For example, if you specify 60, MediaConnect uses 60/1 as the exactFramerate.\"\n        }\n      ]\n    },\n    \"Par\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"par\"\n          },\n          \"description\": \"The pixel aspect ratio (PAR) of the video.\"\n        }\n      ]\n    },\n    \"Range\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Range\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"range\"\n\
  \          },\n          \"description\": \"The encoding range of the video.\"\n        }\n      ]\n    },\n    \"ScanMode\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ScanMode\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"scanMode\"\n          },\n          \"description\": \"The type of compression that was used to smooth the video\\u2019s appearance.\"\n        }\n      ]\n    },\n    \"Tcs\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Tcs\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"tcs\"\n          },\n          \"description\": \"The transfer characteristic system (TCS) that is used in the video.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconnect/refs/heads/main/json-schema/mediaconnect-api-fmtp-request-schema.json
tags:
- AWS
- Broadcasting
- Live Video
- Media
- Media Transport
title: FmtpRequest
---
