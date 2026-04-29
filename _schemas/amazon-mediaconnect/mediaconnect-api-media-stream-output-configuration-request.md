---
description: The media stream that you want to associate with the output, and the parameters for that association.
layout: schema
name: MediaStreamOutputConfigurationRequest
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
schema_file: json-schema/mediaconnect-api-media-stream-output-configuration-request-schema.json
slug: mediaconnect-api-media-stream-output-configuration-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconnect/refs/heads/main/json-schema/mediaconnect-api-media-stream-output-configuration-request-schema.json\",\n  \"title\": \"MediaStreamOutputConfigurationRequest\",\n  \"description\": \"The media stream that you want to associate with the output, and the parameters for that association.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"DestinationConfigurations\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__listOfDestinationConfigurationRequest\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"destinationConfigurations\"\n          },\n          \"description\": \"The transport parameters that you want to associate with the media stream.\"\n        }\n      ]\n    },\n    \"EncodingName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EncodingName\"\
  \n        },\n        {\n          \"xml\": {\n            \"name\": \"encodingName\"\n          },\n          \"description\": \"The format that will be used to encode the data. For ancillary data streams, set the encoding name to smpte291. For audio streams, set the encoding name to pcm. For video, 2110 streams, set the encoding name to raw. For video, JPEG XS streams, set the encoding name to jxsv.\"\n        }\n      ]\n    },\n    \"EncodingParameters\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EncodingParametersRequest\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"encodingParameters\"\n          },\n          \"description\": \"A collection of parameters that determine how MediaConnect will convert the content. These fields only apply to outputs on flows that have a CDI source.\"\n        }\n      ]\n    },\n    \"MediaStreamName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\
  \n        },\n        {\n          \"xml\": {\n            \"name\": \"mediaStreamName\"\n          },\n          \"description\": \"The name of the media stream that is associated with the output.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"MediaStreamName\",\n    \"EncodingName\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconnect/refs/heads/main/json-schema/mediaconnect-api-media-stream-output-configuration-request-schema.json
tags:
- AWS
- Broadcasting
- Live Video
- Media
- Media Transport
title: MediaStreamOutputConfigurationRequest
---
