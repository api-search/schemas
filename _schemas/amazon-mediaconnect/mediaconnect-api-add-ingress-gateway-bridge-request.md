---
description: AddIngressGatewayBridgeRequest schema from AWS Elemental MediaConnect API
layout: schema
name: AddIngressGatewayBridgeRequest
properties_list:
- description: ''
  name: MaxBitrate
  type: object
- description: ''
  name: MaxOutputs
  type: object
provider_name: Amazon MediaConnect
provider_slug: amazon-mediaconnect
schema_file: json-schema/mediaconnect-api-add-ingress-gateway-bridge-request-schema.json
slug: mediaconnect-api-add-ingress-gateway-bridge-request
source_filename: mediaconnect-api-add-ingress-gateway-bridge-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconnect/refs/heads/main/json-schema/mediaconnect-api-add-ingress-gateway-bridge-request-schema.json\",\n  \"title\": \"AddIngressGatewayBridgeRequest\",\n  \"description\": \"AddIngressGatewayBridgeRequest schema from AWS Elemental MediaConnect API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"MaxBitrate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integer\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"maxBitrate\"\n          },\n          \"description\": \"The maximum expected bitrate (in bps).\"\n        }\n      ]\n    },\n    \"MaxOutputs\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integer\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"maxOutputs\"\n          },\n          \"description\": \"The\
  \ maximum number of expected outputs.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"MaxOutputs\",\n    \"MaxBitrate\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconnect/refs/heads/main/json-schema/mediaconnect-api-add-ingress-gateway-bridge-request-schema.json
tags:
- AWS
- Broadcasting
- Live Video
- Media
- Media Transport
title: AddIngressGatewayBridgeRequest
---
