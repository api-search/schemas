---
description: The settings for a gateway, including its networks.
layout: schema
name: Gateway
properties_list:
- description: ''
  name: EgressCidrBlocks
  type: object
- description: ''
  name: GatewayArn
  type: object
- description: ''
  name: GatewayMessages
  type: object
- description: ''
  name: GatewayState
  type: object
- description: ''
  name: Name
  type: object
- description: ''
  name: Networks
  type: object
provider_name: Amazon MediaConnect
provider_slug: amazon-mediaconnect
schema_file: json-schema/mediaconnect-api-gateway-schema.json
slug: mediaconnect-api-gateway
source_filename: mediaconnect-api-gateway-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconnect/refs/heads/main/json-schema/mediaconnect-api-gateway-schema.json\",\n  \"title\": \"Gateway\",\n  \"description\": \"The settings for a gateway, including its networks.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"EgressCidrBlocks\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__listOf__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"egressCidrBlocks\"\n          },\n          \"description\": \"The range of IP addresses that contribute content or initiate output requests for flows communicating with this gateway. These IP addresses should be in the form of a Classless Inter-Domain Routing (CIDR) block; for example, 10.0.0.0/16.\"\n        }\n      ]\n    },\n    \"GatewayArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\
  \n        },\n        {\n          \"xml\": {\n            \"name\": \"gatewayArn\"\n          },\n          \"description\": \"The Amazon Resource Name (ARN) of the gateway.\"\n        }\n      ]\n    },\n    \"GatewayMessages\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__listOfMessageDetail\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"gatewayMessages\"\n          }\n        }\n      ]\n    },\n    \"GatewayState\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GatewayState\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"gatewayState\"\n          },\n          \"description\": \"The current status of the gateway.\"\n        }\n      ]\n    },\n    \"Name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"name\"\n          },\n          \"description\": \"The name\
  \ of the gateway. This name can not be modified after the gateway is created.\"\n        }\n      ]\n    },\n    \"Networks\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__listOfGatewayNetwork\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"networks\"\n          },\n          \"description\": \"The list of networks in the gateway.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"GatewayArn\",\n    \"Networks\",\n    \"EgressCidrBlocks\",\n    \"Name\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconnect/refs/heads/main/json-schema/mediaconnect-api-gateway-schema.json
tags:
- Broadcasting
- Live Video
- Media
- Media Transport
title: Gateway
---
