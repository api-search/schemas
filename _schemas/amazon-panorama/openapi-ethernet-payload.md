---
description: A device's network configuration.
layout: schema
name: EthernetPayload
properties_list:
- description: ''
  name: ConnectionType
  type: object
- description: ''
  name: StaticIpConnectionInfo
  type: object
provider_name: Amazon Panorama
provider_slug: amazon-panorama
schema_file: json-schema/openapi-ethernet-payload-schema.json
slug: openapi-ethernet-payload
source_filename: openapi-ethernet-payload-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-panorama/refs/heads/main/json-schema/openapi-ethernet-payload-schema.json\",\n  \"title\": \"EthernetPayload\",\n  \"description\": \"A device's network configuration.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ConnectionType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ConnectionType\"\n        },\n        {\n          \"description\": \"How the device gets an IP address.\"\n        }\n      ]\n    },\n    \"StaticIpConnectionInfo\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StaticIpConnectionInfo\"\n        },\n        {\n          \"description\": \"Network configuration for a static IP connection.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"ConnectionType\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-panorama/refs/heads/main/json-schema/openapi-ethernet-payload-schema.json
tags:
- AWS
- Cameras
- Computer Vision
- Edge ML
- Industrial IoT
title: EthernetPayload
---
