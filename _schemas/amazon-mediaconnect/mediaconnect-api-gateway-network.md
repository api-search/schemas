---
description: The network settings for a gateway.
layout: schema
name: GatewayNetwork
properties_list:
- description: ''
  name: CidrBlock
  type: object
- description: ''
  name: Name
  type: object
provider_name: Amazon MediaConnect
provider_slug: amazon-mediaconnect
schema_file: json-schema/mediaconnect-api-gateway-network-schema.json
slug: mediaconnect-api-gateway-network
source_filename: mediaconnect-api-gateway-network-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconnect/refs/heads/main/json-schema/mediaconnect-api-gateway-network-schema.json\",\n  \"title\": \"GatewayNetwork\",\n  \"description\": \"The network settings for a gateway.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"CidrBlock\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"cidrBlock\"\n          },\n          \"description\": \"A unique IP address range to use for this network. These IP addresses should be in the form of a Classless Inter-Domain Routing (CIDR) block; for example, 10.0.0.0/16.\"\n        }\n      ]\n    },\n    \"Name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"name\"\n      \
  \    },\n          \"description\": \"The name of the network. This name is used to reference the network and must be unique among networks in this gateway.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"CidrBlock\",\n    \"Name\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconnect/refs/heads/main/json-schema/mediaconnect-api-gateway-network-schema.json
tags:
- AWS
- Broadcasting
- Live Video
- Media
- Media Transport
title: GatewayNetwork
---
