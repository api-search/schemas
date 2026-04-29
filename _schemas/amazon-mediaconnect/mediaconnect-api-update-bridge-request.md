---
description: A request to update the bridge.
layout: schema
name: UpdateBridgeRequest
properties_list:
- description: ''
  name: EgressGatewayBridge
  type: object
- description: ''
  name: IngressGatewayBridge
  type: object
- description: ''
  name: SourceFailoverConfig
  type: object
provider_name: Amazon MediaConnect
provider_slug: amazon-mediaconnect
schema_file: json-schema/mediaconnect-api-update-bridge-request-schema.json
slug: mediaconnect-api-update-bridge-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconnect/refs/heads/main/json-schema/mediaconnect-api-update-bridge-request-schema.json\",\n  \"title\": \"UpdateBridgeRequest\",\n  \"description\": \"A request to update the bridge.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"EgressGatewayBridge\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UpdateEgressGatewayBridgeRequest\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"egressGatewayBridge\"\n          }\n        }\n      ]\n    },\n    \"IngressGatewayBridge\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UpdateIngressGatewayBridgeRequest\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"ingressGatewayBridge\"\n          }\n        }\n      ]\n    },\n    \"SourceFailoverConfig\": {\n      \"allOf\": [\n     \
  \   {\n          \"$ref\": \"#/components/schemas/UpdateFailoverConfig\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"sourceFailoverConfig\"\n          }\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconnect/refs/heads/main/json-schema/mediaconnect-api-update-bridge-request-schema.json
tags:
- AWS
- Broadcasting
- Live Video
- Media
- Media Transport
title: UpdateBridgeRequest
---
