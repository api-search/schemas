---
description: The network configuration for a device.
layout: schema
name: NetworkPayload
properties_list:
- description: ''
  name: Ethernet0
  type: object
- description: ''
  name: Ethernet1
  type: object
- description: ''
  name: Ntp
  type: object
provider_name: Amazon Panorama
provider_slug: amazon-panorama
schema_file: json-schema/openapi-network-payload-schema.json
slug: openapi-network-payload
source_filename: openapi-network-payload-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-panorama/refs/heads/main/json-schema/openapi-network-payload-schema.json\",\n  \"title\": \"NetworkPayload\",\n  \"description\": \"The network configuration for a device.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Ethernet0\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EthernetPayload\"\n        },\n        {\n          \"description\": \"Settings for Ethernet port 0.\"\n        }\n      ]\n    },\n    \"Ethernet1\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EthernetPayload\"\n        },\n        {\n          \"description\": \"Settings for Ethernet port 1.\"\n        }\n      ]\n    },\n    \"Ntp\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NtpPayload\"\n        },\n        {\n          \"description\": \"Network time protocol\
  \ (NTP) server settings.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-panorama/refs/heads/main/json-schema/openapi-network-payload-schema.json
tags:
- Cameras
- Computer Vision
- Edge ML
- Industrial IoT
title: NetworkPayload
---
