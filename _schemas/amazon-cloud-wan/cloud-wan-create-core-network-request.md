---
description: Request body for creating a core network.
layout: schema
name: CreateCoreNetworkRequest
properties_list:
- description: The ID of the global network that a core network will be a part of.
  name: GlobalNetworkId
  type: string
- description: The description of a core network.
  name: Description
  type: string
- description: Key-value tags for the core network.
  name: Tags
  type: array
provider_name: Amazon Cloud WAN
provider_slug: amazon-cloud-wan
schema_file: json-schema/cloud-wan-create-core-network-request-schema.json
slug: cloud-wan-create-core-network-request
source_filename: cloud-wan-create-core-network-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-cloud-wan/refs/heads/main/json-schema/cloud-wan-create-core-network-request-schema.json\",\n  \"title\": \"CreateCoreNetworkRequest\",\n  \"description\": \"Request body for creating a core network.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"GlobalNetworkId\": {\n      \"type\": \"string\",\n      \"description\": \"The ID of the global network that a core network will be a part of.\",\n      \"example\": \"global-network-abc12345\"\n    },\n    \"Description\": {\n      \"type\": \"string\",\n      \"description\": \"The description of a core network.\"\n    },\n    \"Tags\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\"\n      },\n      \"description\": \"Key-value tags for the core network.\"\n    }\n  },\n  \"required\": [\n    \"GlobalNetworkId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-cloud-wan/refs/heads/main/json-schema/cloud-wan-create-core-network-request-schema.json
tags:
- AWS
- Cloud WAN
- Networking
- Wide Area Network
- SD-WAN
title: CreateCoreNetworkRequest
---
