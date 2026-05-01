---
description: EgressGatewayBridge schema from AWS Elemental MediaConnect API
layout: schema
name: EgressGatewayBridge
properties_list:
- description: ''
  name: InstanceId
  type: object
- description: ''
  name: MaxBitrate
  type: object
provider_name: Amazon MediaConnect
provider_slug: amazon-mediaconnect
schema_file: json-schema/mediaconnect-api-egress-gateway-bridge-schema.json
slug: mediaconnect-api-egress-gateway-bridge
source_filename: mediaconnect-api-egress-gateway-bridge-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconnect/refs/heads/main/json-schema/mediaconnect-api-egress-gateway-bridge-schema.json\",\n  \"title\": \"EgressGatewayBridge\",\n  \"description\": \"EgressGatewayBridge schema from AWS Elemental MediaConnect API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"InstanceId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"instanceId\"\n          },\n          \"description\": \"The ID of the instance running this bridge.\"\n        }\n      ]\n    },\n    \"MaxBitrate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integer\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"maxBitrate\"\n          },\n          \"description\": \"The maximum expected bitrate (in bps)\
  \ of the egress bridge.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"MaxBitrate\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconnect/refs/heads/main/json-schema/mediaconnect-api-egress-gateway-bridge-schema.json
tags:
- Broadcasting
- Live Video
- Media
- Media Transport
title: EgressGatewayBridge
---
