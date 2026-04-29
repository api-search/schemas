---
description: A static IP configuration.
layout: schema
name: StaticIpConnectionInfo
properties_list:
- description: ''
  name: DefaultGateway
  type: object
- description: ''
  name: Dns
  type: object
- description: ''
  name: IpAddress
  type: object
- description: ''
  name: Mask
  type: object
provider_name: Amazon Panorama
provider_slug: amazon-panorama
schema_file: json-schema/openapi-static-ip-connection-info-schema.json
slug: openapi-static-ip-connection-info
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-panorama/refs/heads/main/json-schema/openapi-static-ip-connection-info-schema.json\",\n  \"title\": \"StaticIpConnectionInfo\",\n  \"description\": \"A static IP configuration.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"DefaultGateway\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DefaultGateway\"\n        },\n        {\n          \"description\": \"The connection's default gateway.\"\n        }\n      ]\n    },\n    \"Dns\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DnsList\"\n        },\n        {\n          \"description\": \"The connection's DNS address.\"\n        }\n      ]\n    },\n    \"IpAddress\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IpAddress\"\n        },\n        {\n          \"description\": \"The connection's\
  \ IP address.\"\n        }\n      ]\n    },\n    \"Mask\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Mask\"\n        },\n        {\n          \"description\": \"The connection's DNS mask.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"DefaultGateway\",\n    \"Dns\",\n    \"IpAddress\",\n    \"Mask\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-panorama/refs/heads/main/json-schema/openapi-static-ip-connection-info-schema.json
tags:
- AWS
- Cameras
- Computer Vision
- Edge ML
- Industrial IoT
title: StaticIpConnectionInfo
---
