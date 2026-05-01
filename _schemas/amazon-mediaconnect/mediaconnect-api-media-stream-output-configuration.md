---
description: The media stream that is associated with the output, and the parameters for that association.
layout: schema
name: MediaStreamOutputConfiguration
properties_list:
- description: ''
  name: DestinationConfigurations
  type: object
- description: ''
  name: EncodingName
  type: object
- description: ''
  name: EncodingParameters
  type: object
- description: ''
  name: MediaStreamName
  type: object
provider_name: Amazon MediaConnect
provider_slug: amazon-mediaconnect
schema_file: json-schema/mediaconnect-api-media-stream-output-configuration-schema.json
slug: mediaconnect-api-media-stream-output-configuration
source_filename: mediaconnect-api-media-stream-output-configuration-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconnect/refs/heads/main/json-schema/mediaconnect-api-media-stream-output-configuration-schema.json\",\n  \"title\": \"MediaStreamOutputConfiguration\",\n  \"description\": \"The media stream that is associated with the output, and the parameters for that association.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"DestinationConfigurations\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__listOfDestinationConfiguration\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"destinationConfigurations\"\n          },\n          \"description\": \"The transport parameters that are associated with each outbound media stream.\"\n        }\n      ]\n    },\n    \"EncodingName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EncodingName\"\n        },\n \
  \       {\n          \"xml\": {\n            \"name\": \"encodingName\"\n          },\n          \"description\": \"The format that was used to encode the data. For ancillary data streams, set the encoding name to smpte291. For audio streams, set the encoding name to pcm. For video, 2110 streams, set the encoding name to raw. For video, JPEG XS streams, set the encoding name to jxsv.\"\n        }\n      ]\n    },\n    \"EncodingParameters\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EncodingParameters\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"encodingParameters\"\n          },\n          \"description\": \"Encoding parameters\"\n        }\n      ]\n    },\n    \"MediaStreamName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"mediaStreamName\"\n          },\n          \"description\": \"The name of the media stream.\"\
  \n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"MediaStreamName\",\n    \"EncodingName\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconnect/refs/heads/main/json-schema/mediaconnect-api-media-stream-output-configuration-schema.json
tags:
- Broadcasting
- Live Video
- Media
- Media Transport
title: MediaStreamOutputConfiguration
---
