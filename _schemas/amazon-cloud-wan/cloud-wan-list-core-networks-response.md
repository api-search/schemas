---
description: Response for listing core networks.
layout: schema
name: ListCoreNetworksResponse
properties_list:
- description: ''
  name: CoreNetworks
  type: array
- description: ''
  name: NextToken
  type: string
provider_name: Amazon Cloud WAN
provider_slug: amazon-cloud-wan
schema_file: json-schema/cloud-wan-list-core-networks-response-schema.json
slug: cloud-wan-list-core-networks-response
source_filename: cloud-wan-list-core-networks-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-cloud-wan/refs/heads/main/json-schema/cloud-wan-list-core-networks-response-schema.json\",\n  \"title\": \"ListCoreNetworksResponse\",\n  \"description\": \"Response for listing core networks.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"CoreNetworks\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/CoreNetwork\"\n      }\n    },\n    \"NextToken\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-cloud-wan/refs/heads/main/json-schema/cloud-wan-list-core-networks-response-schema.json
tags:
- Cloud WAN
- Networking
- Wide Area Network
- SD-WAN
title: ListCoreNetworksResponse
---
