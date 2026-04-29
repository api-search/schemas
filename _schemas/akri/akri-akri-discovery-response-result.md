---
description: Counter for Discovery Handler success and failure responses
layout: schema
name: AkriDiscoveryResponseResult
properties_list:
- description: Name of the Akri Configuration resource
  name: configuration
  type: string
- description: Result of the discovery response
  name: result
  type: string
- description: Total count of responses
  name: value
  type: number
provider_name: Akri
provider_slug: akri
schema_file: json-schema/akri-akri-discovery-response-result-schema.json
slug: akri-akri-discovery-response-result
source_filename: akri-akri-discovery-response-result-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/akri/refs/heads/main/json-schema/akri-akri-discovery-response-result-schema.json\",\n  \"title\": \"AkriDiscoveryResponseResult\",\n  \"description\": \"Counter for Discovery Handler success and failure responses\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"configuration\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the Akri Configuration resource\",\n      \"example\": \"onvif-camera\"\n    },\n    \"result\": {\n      \"type\": \"string\",\n      \"description\": \"Result of the discovery response\",\n      \"enum\": [\n        \"success\",\n        \"failure\"\n      ],\n      \"example\": \"success\"\n    },\n    \"value\": {\n      \"type\": \"number\",\n      \"description\": \"Total count of responses\",\n      \"example\": 42\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/akri/refs/heads/main/json-schema/akri-akri-discovery-response-result-schema.json
tags:
- Device Management
- Edge Computing
- IoT
- Kubernetes
- CNCF
- Open Source
- OPC UA
- ONVIF
- udev
title: AkriDiscoveryResponseResult
---
