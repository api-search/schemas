---
description: The transport parameters that you want to associate with an outbound media stream.
layout: schema
name: DestinationConfigurationRequest
properties_list:
- description: ''
  name: DestinationIp
  type: object
- description: ''
  name: DestinationPort
  type: object
- description: ''
  name: Interface
  type: object
provider_name: Amazon MediaConnect
provider_slug: amazon-mediaconnect
schema_file: json-schema/mediaconnect-api-destination-configuration-request-schema.json
slug: mediaconnect-api-destination-configuration-request
source_filename: mediaconnect-api-destination-configuration-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconnect/refs/heads/main/json-schema/mediaconnect-api-destination-configuration-request-schema.json\",\n  \"title\": \"DestinationConfigurationRequest\",\n  \"description\": \"The transport parameters that you want to associate with an outbound media stream.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"DestinationIp\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"destinationIp\"\n          },\n          \"description\": \"The IP address where you want MediaConnect to send contents of the media stream.\"\n        }\n      ]\n    },\n    \"DestinationPort\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integer\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"\
  destinationPort\"\n          },\n          \"description\": \"The port that you want MediaConnect to use when it distributes the media stream to the output.\"\n        }\n      ]\n    },\n    \"Interface\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/InterfaceRequest\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"interface\"\n          },\n          \"description\": \"The VPC interface that you want to use for the media stream associated with the output.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"DestinationIp\",\n    \"DestinationPort\",\n    \"Interface\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconnect/refs/heads/main/json-schema/mediaconnect-api-destination-configuration-request-schema.json
tags:
- Broadcasting
- Live Video
- Media
- Media Transport
title: DestinationConfigurationRequest
---
