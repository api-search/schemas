---
description: The network status of a device.
layout: schema
name: NetworkStatus
properties_list:
- description: ''
  name: Ethernet0Status
  type: object
- description: ''
  name: Ethernet1Status
  type: object
- description: ''
  name: LastUpdatedTime
  type: object
- description: ''
  name: NtpStatus
  type: object
provider_name: Amazon Panorama
provider_slug: amazon-panorama
schema_file: json-schema/openapi-network-status-schema.json
slug: openapi-network-status
source_filename: openapi-network-status-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-panorama/refs/heads/main/json-schema/openapi-network-status-schema.json\",\n  \"title\": \"NetworkStatus\",\n  \"description\": \"The network status of a device.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Ethernet0Status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EthernetStatus\"\n        },\n        {\n          \"description\": \"The status of Ethernet port 0.\"\n        }\n      ]\n    },\n    \"Ethernet1Status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EthernetStatus\"\n        },\n        {\n          \"description\": \"The status of Ethernet port 1.\"\n        }\n      ]\n    },\n    \"LastUpdatedTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LastUpdatedTime\"\n        },\n        {\n          \"description\"\
  : \"When the network status changed.\"\n        }\n      ]\n    },\n    \"NtpStatus\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NtpStatus\"\n        },\n        {\n          \"description\": \"Details about a network time protocol (NTP) server connection.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-panorama/refs/heads/main/json-schema/openapi-network-status-schema.json
tags:
- AWS
- Cameras
- Computer Vision
- Edge ML
- Industrial IoT
title: NetworkStatus
---
