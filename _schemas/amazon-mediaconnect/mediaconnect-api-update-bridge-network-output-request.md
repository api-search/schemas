---
description: Update an existing network output.
layout: schema
name: UpdateBridgeNetworkOutputRequest
properties_list:
- description: ''
  name: IpAddress
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
- description: ''
  name: Ttl
  type: object
provider_name: Amazon MediaConnect
provider_slug: amazon-mediaconnect
schema_file: json-schema/mediaconnect-api-update-bridge-network-output-request-schema.json
slug: mediaconnect-api-update-bridge-network-output-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconnect/refs/heads/main/json-schema/mediaconnect-api-update-bridge-network-output-request-schema.json\",\n  \"title\": \"UpdateBridgeNetworkOutputRequest\",\n  \"description\": \"Update an existing network output.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"IpAddress\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"ipAddress\"\n          },\n          \"description\": \"The network output IP Address.\"\n        }\n      ]\n    },\n    \"NetworkName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"networkName\"\n          },\n          \"description\": \"The network output's gateway network name.\"\n  \
  \      }\n      ]\n    },\n    \"Port\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integer\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"port\"\n          },\n          \"description\": \"The network output port.\"\n        }\n      ]\n    },\n    \"Protocol\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Protocol\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"protocol\"\n          },\n          \"description\": \"The network output protocol.\"\n        }\n      ]\n    },\n    \"Ttl\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integer\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"ttl\"\n          },\n          \"description\": \"The network output TTL.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconnect/refs/heads/main/json-schema/mediaconnect-api-update-bridge-network-output-request-schema.json
tags:
- AWS
- Broadcasting
- Live Video
- Media
- Media Transport
title: UpdateBridgeNetworkOutputRequest
---
