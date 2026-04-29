---
description: Response for getting a core network.
layout: schema
name: GetCoreNetworkResponse
properties_list:
- description: ''
  name: CoreNetwork
  type: object
provider_name: Amazon Cloud WAN
provider_slug: amazon-cloud-wan
schema_file: json-schema/cloud-wan-get-core-network-response-schema.json
slug: cloud-wan-get-core-network-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-cloud-wan/refs/heads/main/json-schema/cloud-wan-get-core-network-response-schema.json\",\n  \"title\": \"GetCoreNetworkResponse\",\n  \"description\": \"Response for getting a core network.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"CoreNetwork\": {\n      \"$ref\": \"#/components/schemas/CoreNetwork\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-cloud-wan/refs/heads/main/json-schema/cloud-wan-get-core-network-response-schema.json
tags:
- AWS
- Cloud WAN
- Networking
- Wide Area Network
- SD-WAN
title: GetCoreNetworkResponse
---
