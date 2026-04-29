---
description: A collection of parameters that determine how MediaConnect will convert the content. These fields only apply to outputs on flows that have a CDI source.
layout: schema
name: EncodingParameters
properties_list:
- description: ''
  name: CompressionFactor
  type: object
- description: ''
  name: EncoderProfile
  type: object
provider_name: Amazon MediaConnect
provider_slug: amazon-mediaconnect
schema_file: json-schema/mediaconnect-api-encoding-parameters-schema.json
slug: mediaconnect-api-encoding-parameters
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconnect/refs/heads/main/json-schema/mediaconnect-api-encoding-parameters-schema.json\",\n  \"title\": \"EncodingParameters\",\n  \"description\": \"A collection of parameters that determine how MediaConnect will convert the content. These fields only apply to outputs on flows that have a CDI source.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"CompressionFactor\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__double\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"compressionFactor\"\n          },\n          \"description\": \"A value that is used to calculate compression for an output. The bitrate of the output is calculated as follows: Output bitrate = (1 / compressionFactor) * (source bitrate) This property only applies to outputs that use the ST 2110 JPEG XS protocol,\
  \ with a flow source that uses the CDI protocol. Valid values are floating point numbers in the range of 3.0 to 10.0, inclusive.\"\n        }\n      ]\n    },\n    \"EncoderProfile\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EncoderProfile\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"encoderProfile\"\n          },\n          \"description\": \"A setting on the encoder that drives compression settings. This property only applies to video media streams associated with outputs that use the ST 2110 JPEG XS protocol, with a flow source that uses the CDI protocol.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"EncoderProfile\",\n    \"CompressionFactor\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconnect/refs/heads/main/json-schema/mediaconnect-api-encoding-parameters-schema.json
tags:
- AWS
- Broadcasting
- Live Video
- Media
- Media Transport
title: EncodingParameters
---
