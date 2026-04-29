---
description: A device's Ethernet status.
layout: schema
name: EthernetStatus
properties_list:
- description: ''
  name: ConnectionStatus
  type: object
- description: ''
  name: HwAddress
  type: object
- description: ''
  name: IpAddress
  type: object
provider_name: Amazon Panorama
provider_slug: amazon-panorama
schema_file: json-schema/openapi-ethernet-status-schema.json
slug: openapi-ethernet-status
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-panorama/refs/heads/main/json-schema/openapi-ethernet-status-schema.json\",\n  \"title\": \"EthernetStatus\",\n  \"description\": \"A device's Ethernet status.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ConnectionStatus\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NetworkConnectionStatus\"\n        },\n        {\n          \"description\": \"The device's connection status.\"\n        }\n      ]\n    },\n    \"HwAddress\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/HwAddress\"\n        },\n        {\n          \"description\": \"The device's physical address.\"\n        }\n      ]\n    },\n    \"IpAddress\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IpAddress\"\n        },\n        {\n          \"description\": \"The device's\
  \ IP address.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-panorama/refs/heads/main/json-schema/openapi-ethernet-status-schema.json
tags:
- AWS
- Cameras
- Computer Vision
- Edge ML
- Industrial IoT
title: EthernetStatus
---
