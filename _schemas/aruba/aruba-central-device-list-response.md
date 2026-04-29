---
description: ''
layout: schema
name: DeviceListResponse
properties_list:
- description: Total number of devices matching the query.
  name: total
  type: integer
- description: Number of devices returned in this response.
  name: count
  type: integer
- description: ''
  name: devices
  type: array
provider_name: Aruba
provider_slug: aruba
schema_file: json-schema/aruba-central-device-list-response-schema.json
slug: aruba-central-device-list-response
source_filename: aruba-central-device-list-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"DeviceListResponse\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"total\": {\n      \"type\": \"integer\",\n      \"description\": \"Total number of devices matching the query.\"\n    },\n    \"count\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of devices returned in this response.\"\n    },\n    \"devices\": {\n      \"type\": \"array\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aruba/refs/heads/main/json-schema/aruba-central-device-list-response-schema.json
tags:
- Cloud
- Infrastructure
- Network Management
- Networking
- SD-WAN
- Security
- Switches
- Wireless
title: DeviceListResponse
---
