---
description: ''
layout: schema
name: NetworkListResponse
properties_list:
- description: Total number of networks.
  name: total
  type: integer
- description: Number of networks returned.
  name: count
  type: integer
- description: ''
  name: networks
  type: array
provider_name: Aruba
provider_slug: aruba
schema_file: json-schema/aruba-central-network-list-response-schema.json
slug: aruba-central-network-list-response
source_filename: aruba-central-network-list-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"NetworkListResponse\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"total\": {\n      \"type\": \"integer\",\n      \"description\": \"Total number of networks.\"\n    },\n    \"count\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of networks returned.\"\n    },\n    \"networks\": {\n      \"type\": \"array\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aruba/refs/heads/main/json-schema/aruba-central-network-list-response-schema.json
tags:
- Cloud
- Infrastructure
- Network Management
- Networking
- SD-WAN
- Security
- Switches
- Wireless
title: NetworkListResponse
---
