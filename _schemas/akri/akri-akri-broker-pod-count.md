---
description: Gauge tracking the number of broker pods per configuration and node
layout: schema
name: AkriBrokerPodCount
properties_list:
- description: Name of the Akri Configuration resource
  name: configuration
  type: string
- description: Kubernetes node name
  name: node
  type: string
- description: Current count of broker pods
  name: value
  type: number
provider_name: Akri
provider_slug: akri
schema_file: json-schema/akri-akri-broker-pod-count-schema.json
slug: akri-akri-broker-pod-count
source_filename: akri-akri-broker-pod-count-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/akri/refs/heads/main/json-schema/akri-akri-broker-pod-count-schema.json\",\n  \"title\": \"AkriBrokerPodCount\",\n  \"description\": \"Gauge tracking the number of broker pods per configuration and node\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"configuration\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the Akri Configuration resource\",\n      \"example\": \"onvif-camera\"\n    },\n    \"node\": {\n      \"type\": \"string\",\n      \"description\": \"Kubernetes node name\",\n      \"example\": \"node-01\"\n    },\n    \"value\": {\n      \"type\": \"number\",\n      \"description\": \"Current count of broker pods\",\n      \"example\": 1\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/akri/refs/heads/main/json-schema/akri-akri-broker-pod-count-schema.json
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
title: AkriBrokerPodCount
---
