---
description: ''
layout: schema
name: GroupListResponse
properties_list:
- description: Total number of groups.
  name: total
  type: integer
- description: Number of groups returned.
  name: count
  type: integer
- description: ''
  name: data
  type: array
provider_name: Aruba
provider_slug: aruba
schema_file: json-schema/aruba-central-group-list-response-schema.json
slug: aruba-central-group-list-response
source_filename: aruba-central-group-list-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"GroupListResponse\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"total\": {\n      \"type\": \"integer\",\n      \"description\": \"Total number of groups.\"\n    },\n    \"count\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of groups returned.\"\n    },\n    \"data\": {\n      \"type\": \"array\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aruba/refs/heads/main/json-schema/aruba-central-group-list-response-schema.json
tags:
- Cloud
- Infrastructure
- Network Management
- Networking
- SD-WAN
- Security
- Switches
- Wireless
title: GroupListResponse
---
