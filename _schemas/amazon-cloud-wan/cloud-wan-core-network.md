---
description: Describes a core network.
layout: schema
name: CoreNetwork
properties_list:
- description: The ID of a core network.
  name: CoreNetworkId
  type: string
- description: The ARN of a core network.
  name: CoreNetworkArn
  type: string
- description: The ID of the global network where a core network is a part of.
  name: GlobalNetworkId
  type: string
- description: The description of a core network.
  name: Description
  type: string
- description: The current state of a core network.
  name: State
  type: string
- description: The timestamp when a core network was created.
  name: CreatedAt
  type: string
provider_name: Amazon Cloud WAN
provider_slug: amazon-cloud-wan
schema_file: json-schema/cloud-wan-core-network-schema.json
slug: cloud-wan-core-network
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-cloud-wan/refs/heads/main/json-schema/cloud-wan-core-network-schema.json\",\n  \"title\": \"CoreNetwork\",\n  \"description\": \"Describes a core network.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"CoreNetworkId\": {\n      \"type\": \"string\",\n      \"description\": \"The ID of a core network.\",\n      \"example\": \"core-network-abc12345\"\n    },\n    \"CoreNetworkArn\": {\n      \"type\": \"string\",\n      \"description\": \"The ARN of a core network.\"\n    },\n    \"GlobalNetworkId\": {\n      \"type\": \"string\",\n      \"description\": \"The ID of the global network where a core network is a part of.\"\n    },\n    \"Description\": {\n      \"type\": \"string\",\n      \"description\": \"The description of a core network.\"\n    },\n    \"State\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"CREATING\"\
  ,\n        \"UPDATING\",\n        \"AVAILABLE\",\n        \"DELETING\"\n      ],\n      \"description\": \"The current state of a core network.\"\n    },\n    \"CreatedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The timestamp when a core network was created.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-cloud-wan/refs/heads/main/json-schema/cloud-wan-core-network-schema.json
tags:
- AWS
- Cloud WAN
- Networking
- Wide Area Network
- SD-WAN
title: CoreNetwork
---
