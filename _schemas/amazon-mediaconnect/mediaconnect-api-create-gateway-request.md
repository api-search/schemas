---
description: Creates a new gateway. The request must include at least one network (up to 4).
layout: schema
name: CreateGatewayRequest
properties_list:
- description: ''
  name: EgressCidrBlocks
  type: object
- description: ''
  name: Name
  type: object
- description: ''
  name: Networks
  type: object
provider_name: Amazon MediaConnect
provider_slug: amazon-mediaconnect
schema_file: json-schema/mediaconnect-api-create-gateway-request-schema.json
slug: mediaconnect-api-create-gateway-request
source_filename: mediaconnect-api-create-gateway-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconnect/refs/heads/main/json-schema/mediaconnect-api-create-gateway-request-schema.json\",\n  \"title\": \"CreateGatewayRequest\",\n  \"description\": \"Creates a new gateway. The request must include at least one network (up to 4).\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"EgressCidrBlocks\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__listOf__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"egressCidrBlocks\"\n          },\n          \"description\": \"The range of IP addresses that are allowed to contribute content or initiate output requests for flows communicating with this gateway. These IP addresses should be in the form of a Classless Inter-Domain Routing (CIDR) block; for example, 10.0.0.0/16.\"\n        }\n      ]\n    },\n    \"Name\": {\n     \
  \ \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"name\"\n          },\n          \"description\": \"The name of the gateway. This name can not be modified after the gateway is created.\"\n        }\n      ]\n    },\n    \"Networks\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__listOfGatewayNetwork\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"networks\"\n          },\n          \"description\": \"The list of networks that you want to add.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Networks\",\n    \"EgressCidrBlocks\",\n    \"Name\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconnect/refs/heads/main/json-schema/mediaconnect-api-create-gateway-request-schema.json
tags:
- AWS
- Broadcasting
- Live Video
- Media
- Media Transport
title: CreateGatewayRequest
---
