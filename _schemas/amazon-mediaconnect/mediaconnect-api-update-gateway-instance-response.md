---
description: UpdateGatewayInstanceResponse schema from AWS Elemental MediaConnect API
layout: schema
name: UpdateGatewayInstanceResponse
properties_list:
- description: ''
  name: BridgePlacement
  type: object
- description: ''
  name: GatewayInstanceArn
  type: object
provider_name: Amazon MediaConnect
provider_slug: amazon-mediaconnect
schema_file: json-schema/mediaconnect-api-update-gateway-instance-response-schema.json
slug: mediaconnect-api-update-gateway-instance-response
source_filename: mediaconnect-api-update-gateway-instance-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconnect/refs/heads/main/json-schema/mediaconnect-api-update-gateway-instance-response-schema.json\",\n  \"title\": \"UpdateGatewayInstanceResponse\",\n  \"description\": \"UpdateGatewayInstanceResponse schema from AWS Elemental MediaConnect API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"BridgePlacement\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BridgePlacement\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"bridgePlacement\"\n          },\n          \"description\": \"The availability of the instance to host new bridges. The bridgePlacement property can be LOCKED or AVAILABLE. If it is LOCKED, no new bridges can be deployed to this instance. If it is AVAILABLE, new bridges can be added to this instance.\"\n        }\n      ]\n    },\n    \"GatewayInstanceArn\"\
  : {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"gatewayInstanceArn\"\n          },\n          \"description\": \"The Amazon Resource Name (ARN) of the instance.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconnect/refs/heads/main/json-schema/mediaconnect-api-update-gateway-instance-response-schema.json
tags:
- Broadcasting
- Live Video
- Media
- Media Transport
title: UpdateGatewayInstanceResponse
---
