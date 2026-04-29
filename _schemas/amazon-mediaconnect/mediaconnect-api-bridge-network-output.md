---
description: The output of the bridge. A network output is delivered to your premises.
layout: schema
name: BridgeNetworkOutput
properties_list:
- description: ''
  name: IpAddress
  type: object
- description: ''
  name: Name
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
schema_file: json-schema/mediaconnect-api-bridge-network-output-schema.json
slug: mediaconnect-api-bridge-network-output
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconnect/refs/heads/main/json-schema/mediaconnect-api-bridge-network-output-schema.json\",\n  \"title\": \"BridgeNetworkOutput\",\n  \"description\": \"The output of the bridge. A network output is delivered to your premises.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"IpAddress\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"ipAddress\"\n          },\n          \"description\": \"The network output IP Address.\"\n        }\n      ]\n    },\n    \"Name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"name\"\n          },\n          \"description\": \"The network output name.\"\n        }\n      ]\n   \
  \ },\n    \"NetworkName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"networkName\"\n          },\n          \"description\": \"The network output's gateway network name.\"\n        }\n      ]\n    },\n    \"Port\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integer\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"port\"\n          },\n          \"description\": \"The network output port.\"\n        }\n      ]\n    },\n    \"Protocol\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Protocol\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"protocol\"\n          },\n          \"description\": \"The network output protocol.\"\n        }\n      ]\n    },\n    \"Ttl\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integer\"\n        },\n\
  \        {\n          \"xml\": {\n            \"name\": \"ttl\"\n          },\n          \"description\": \"The network output TTL.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"NetworkName\",\n    \"Port\",\n    \"IpAddress\",\n    \"Protocol\",\n    \"Ttl\",\n    \"Name\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconnect/refs/heads/main/json-schema/mediaconnect-api-bridge-network-output-schema.json
tags:
- AWS
- Broadcasting
- Live Video
- Media
- Media Transport
title: BridgeNetworkOutput
---
