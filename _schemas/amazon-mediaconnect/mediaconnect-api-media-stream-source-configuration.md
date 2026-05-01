---
description: The media stream that is associated with the source, and the parameters for that association.
layout: schema
name: MediaStreamSourceConfiguration
properties_list:
- description: ''
  name: EncodingName
  type: object
- description: ''
  name: InputConfigurations
  type: object
- description: ''
  name: MediaStreamName
  type: object
provider_name: Amazon MediaConnect
provider_slug: amazon-mediaconnect
schema_file: json-schema/mediaconnect-api-media-stream-source-configuration-schema.json
slug: mediaconnect-api-media-stream-source-configuration
source_filename: mediaconnect-api-media-stream-source-configuration-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconnect/refs/heads/main/json-schema/mediaconnect-api-media-stream-source-configuration-schema.json\",\n  \"title\": \"MediaStreamSourceConfiguration\",\n  \"description\": \"The media stream that is associated with the source, and the parameters for that association.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"EncodingName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EncodingName\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"encodingName\"\n          },\n          \"description\": \"The format that was used to encode the data. For ancillary data streams, set the encoding name to smpte291. For audio streams, set the encoding name to pcm. For video, 2110 streams, set the encoding name to raw. For video, JPEG XS streams, set the encoding name to jxsv.\"\n        }\n\
  \      ]\n    },\n    \"InputConfigurations\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__listOfInputConfiguration\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"inputConfigurations\"\n          },\n          \"description\": \"The transport parameters that are associated with an incoming media stream.\"\n        }\n      ]\n    },\n    \"MediaStreamName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"mediaStreamName\"\n          },\n          \"description\": \"The name of the media stream.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"MediaStreamName\",\n    \"EncodingName\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconnect/refs/heads/main/json-schema/mediaconnect-api-media-stream-source-configuration-schema.json
tags:
- Broadcasting
- Live Video
- Media
- Media Transport
title: MediaStreamSourceConfiguration
---
