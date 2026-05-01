---
description: UpdateEgressGatewayBridgeRequest schema from AWS Elemental MediaConnect API
layout: schema
name: UpdateEgressGatewayBridgeRequest
properties_list:
- description: ''
  name: MaxBitrate
  type: object
provider_name: Amazon MediaConnect
provider_slug: amazon-mediaconnect
schema_file: json-schema/mediaconnect-api-update-egress-gateway-bridge-request-schema.json
slug: mediaconnect-api-update-egress-gateway-bridge-request
source_filename: mediaconnect-api-update-egress-gateway-bridge-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconnect/refs/heads/main/json-schema/mediaconnect-api-update-egress-gateway-bridge-request-schema.json\",\n  \"title\": \"UpdateEgressGatewayBridgeRequest\",\n  \"description\": \"UpdateEgressGatewayBridgeRequest schema from AWS Elemental MediaConnect API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"MaxBitrate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integer\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"maxBitrate\"\n          },\n          \"description\": \"Update an existing egress-type bridge.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconnect/refs/heads/main/json-schema/mediaconnect-api-update-egress-gateway-bridge-request-schema.json
tags:
- Broadcasting
- Live Video
- Media
- Media Transport
title: UpdateEgressGatewayBridgeRequest
---
