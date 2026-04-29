---
description: The transport parameters that are associated with an outbound media stream.
layout: schema
name: DestinationConfiguration
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
- description: ''
  name: OutboundIp
  type: object
provider_name: Amazon MediaConnect
provider_slug: amazon-mediaconnect
schema_file: json-schema/mediaconnect-api-destination-configuration-schema.json
slug: mediaconnect-api-destination-configuration
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconnect/refs/heads/main/json-schema/mediaconnect-api-destination-configuration-schema.json\",\n  \"title\": \"DestinationConfiguration\",\n  \"description\": \"The transport parameters that are associated with an outbound media stream.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"DestinationIp\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"destinationIp\"\n          },\n          \"description\": \"The IP address where contents of the media stream will be sent.\"\n        }\n      ]\n    },\n    \"DestinationPort\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integer\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"destinationPort\"\n          },\n     \
  \     \"description\": \"The port to use when the content of the media stream is distributed to the output.\"\n        }\n      ]\n    },\n    \"Interface\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Interface\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"interface\"\n          },\n          \"description\": \"The VPC interface that is used for the media stream associated with the output.\"\n        }\n      ]\n    },\n    \"OutboundIp\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"outboundIp\"\n          },\n          \"description\": \"The IP address that the receiver requires in order to establish a connection with the flow. This value is represented by the elastic network interface IP address of the VPC. This field applies only to outputs that use the CDI or ST 2110 JPEG XS protocol.\"\n        }\n      ]\n  \
  \  }\n  },\n  \"required\": [\n    \"DestinationIp\",\n    \"DestinationPort\",\n    \"Interface\",\n    \"OutboundIp\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconnect/refs/heads/main/json-schema/mediaconnect-api-destination-configuration-schema.json
tags:
- AWS
- Broadcasting
- Live Video
- Media
- Media Transport
title: DestinationConfiguration
---
