---
description: Gauge tracking the number of discovered Akri instances per configuration
layout: schema
name: AkriInstanceCount
properties_list:
- description: Name of the Akri Configuration resource
  name: configuration
  type: string
- description: Whether the device is shared across multiple nodes
  name: shared
  type: string
- description: Current count of discovered instances
  name: value
  type: number
provider_name: Akri
provider_slug: akri
schema_file: json-schema/akri-akri-instance-count-schema.json
slug: akri-akri-instance-count
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/akri/refs/heads/main/json-schema/akri-akri-instance-count-schema.json\",\n  \"title\": \"AkriInstanceCount\",\n  \"description\": \"Gauge tracking the number of discovered Akri instances per configuration\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"configuration\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the Akri Configuration resource\",\n      \"example\": \"onvif-camera\"\n    },\n    \"shared\": {\n      \"type\": \"string\",\n      \"description\": \"Whether the device is shared across multiple nodes\",\n      \"example\": \"false\"\n    },\n    \"value\": {\n      \"type\": \"number\",\n      \"description\": \"Current count of discovered instances\",\n      \"example\": 3\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/akri/refs/heads/main/json-schema/akri-akri-instance-count-schema.json
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
title: AkriInstanceCount
---
