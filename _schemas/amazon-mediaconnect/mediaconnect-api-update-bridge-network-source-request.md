---
description: Update the network source of the bridge.
layout: schema
name: UpdateBridgeNetworkSourceRequest
properties_list:
- description: ''
  name: MulticastIp
  type: object
- description: ''
  name: NetworkName
  type: object
- description: ''
  name: Port
  type: object
- description: ''
  name: Protocol
  type: object
provider_name: Amazon MediaConnect
provider_slug: amazon-mediaconnect
schema_file: json-schema/mediaconnect-api-update-bridge-network-source-request-schema.json
slug: mediaconnect-api-update-bridge-network-source-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconnect/refs/heads/main/json-schema/mediaconnect-api-update-bridge-network-source-request-schema.json\",\n  \"title\": \"UpdateBridgeNetworkSourceRequest\",\n  \"description\": \"Update the network source of the bridge.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"MulticastIp\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"multicastIp\"\n          },\n          \"description\": \"The network source multicast IP.\"\n        }\n      ]\n    },\n    \"NetworkName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"networkName\"\n          },\n          \"description\": \"The network source's gateway network\
  \ name.\"\n        }\n      ]\n    },\n    \"Port\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integer\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"port\"\n          },\n          \"description\": \"The network source port.\"\n        }\n      ]\n    },\n    \"Protocol\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Protocol\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"protocol\"\n          },\n          \"description\": \"The network source protocol.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconnect/refs/heads/main/json-schema/mediaconnect-api-update-bridge-network-source-request-schema.json
tags:
- AWS
- Broadcasting
- Live Video
- Media
- Media Transport
title: UpdateBridgeNetworkSourceRequest
---
