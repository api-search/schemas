---
description: The source of the bridge. A network source originates at your premises.
layout: schema
name: BridgeNetworkSource
properties_list:
- description: ''
  name: MulticastIp
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
provider_name: Amazon MediaConnect
provider_slug: amazon-mediaconnect
schema_file: json-schema/mediaconnect-api-bridge-network-source-schema.json
slug: mediaconnect-api-bridge-network-source
source_filename: mediaconnect-api-bridge-network-source-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconnect/refs/heads/main/json-schema/mediaconnect-api-bridge-network-source-schema.json\",\n  \"title\": \"BridgeNetworkSource\",\n  \"description\": \"The source of the bridge. A network source originates at your premises.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"MulticastIp\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"multicastIp\"\n          },\n          \"description\": \"The network source multicast IP.\"\n        }\n      ]\n    },\n    \"Name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"name\"\n          },\n          \"description\": \"The name of the network source.\"\n        }\n \
  \     ]\n    },\n    \"NetworkName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"networkName\"\n          },\n          \"description\": \"The network source's gateway network name.\"\n        }\n      ]\n    },\n    \"Port\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integer\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"port\"\n          },\n          \"description\": \"The network source port.\"\n        }\n      ]\n    },\n    \"Protocol\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Protocol\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"protocol\"\n          },\n          \"description\": \"The network source protocol.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"NetworkName\",\n    \"MulticastIp\",\n    \"Port\",\n    \"Protocol\",\n\
  \    \"Name\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconnect/refs/heads/main/json-schema/mediaconnect-api-bridge-network-source-schema.json
tags:
- AWS
- Broadcasting
- Live Video
- Media
- Media Transport
title: BridgeNetworkSource
---
