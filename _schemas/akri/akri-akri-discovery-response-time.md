---
description: Histogram of Discovery Handler response latency in seconds
layout: schema
name: AkriDiscoveryResponseTime
properties_list:
- description: Name of the Akri Configuration resource
  name: configuration
  type: string
- description: Histogram bucket upper bound in seconds
  name: le
  type: string
- description: Count of observations within this bucket
  name: value
  type: number
provider_name: Akri
provider_slug: akri
schema_file: json-schema/akri-akri-discovery-response-time-schema.json
slug: akri-akri-discovery-response-time
source_filename: akri-akri-discovery-response-time-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/akri/refs/heads/main/json-schema/akri-akri-discovery-response-time-schema.json\",\n  \"title\": \"AkriDiscoveryResponseTime\",\n  \"description\": \"Histogram of Discovery Handler response latency in seconds\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"configuration\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the Akri Configuration resource\",\n      \"example\": \"onvif-camera\"\n    },\n    \"le\": {\n      \"type\": \"string\",\n      \"description\": \"Histogram bucket upper bound in seconds\",\n      \"example\": \"0.005\"\n    },\n    \"value\": {\n      \"type\": \"number\",\n      \"description\": \"Count of observations within this bucket\",\n      \"example\": 10\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/akri/refs/heads/main/json-schema/akri-akri-discovery-response-time-schema.json
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
title: AkriDiscoveryResponseTime
---
