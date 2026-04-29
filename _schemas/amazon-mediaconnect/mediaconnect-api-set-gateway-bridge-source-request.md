---
description: The source configuration for cloud flows receiving a stream from a bridge.
layout: schema
name: SetGatewayBridgeSourceRequest
properties_list:
- description: ''
  name: BridgeArn
  type: object
- description: ''
  name: VpcInterfaceAttachment
  type: object
provider_name: Amazon MediaConnect
provider_slug: amazon-mediaconnect
schema_file: json-schema/mediaconnect-api-set-gateway-bridge-source-request-schema.json
slug: mediaconnect-api-set-gateway-bridge-source-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconnect/refs/heads/main/json-schema/mediaconnect-api-set-gateway-bridge-source-request-schema.json\",\n  \"title\": \"SetGatewayBridgeSourceRequest\",\n  \"description\": \"The source configuration for cloud flows receiving a stream from a bridge.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"BridgeArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"pattern\": \"^arn:.+:mediaconnect.+:bridge:.+$\",\n          \"xml\": {\n            \"name\": \"bridgeArn\"\n          },\n          \"description\": \"The ARN of the bridge feeding this flow.\"\n        }\n      ]\n    },\n    \"VpcInterfaceAttachment\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/VpcInterfaceAttachment\"\n        },\n        {\n          \"xml\": {\n\
  \            \"name\": \"vpcInterfaceAttachment\"\n          },\n          \"description\": \"The name of the VPC interface attachment to use for this bridge source.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"BridgeArn\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconnect/refs/heads/main/json-schema/mediaconnect-api-set-gateway-bridge-source-request-schema.json
tags:
- AWS
- Broadcasting
- Live Video
- Media
- Media Transport
title: SetGatewayBridgeSourceRequest
---
