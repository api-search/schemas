---
description: ''
layout: schema
name: AccessPointListResponse
properties_list:
- description: Total number of access points matching the query.
  name: total
  type: integer
- description: Number of access points returned.
  name: count
  type: integer
- description: ''
  name: aps
  type: array
provider_name: Aruba
provider_slug: aruba
schema_file: json-schema/aruba-central-access-point-list-response-schema.json
slug: aruba-central-access-point-list-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"AccessPointListResponse\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"total\": {\n      \"type\": \"integer\",\n      \"description\": \"Total number of access points matching the query.\"\n    },\n    \"count\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of access points returned.\"\n    },\n    \"aps\": {\n      \"type\": \"array\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aruba/refs/heads/main/json-schema/aruba-central-access-point-list-response-schema.json
tags:
- Cloud
- Infrastructure
- Network Management
- Networking
- SD-WAN
- Security
- Switches
- Wireless
title: AccessPointListResponse
---
