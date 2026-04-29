---
description: Details about an NTP server connection.
layout: schema
name: NtpStatus
properties_list:
- description: ''
  name: ConnectionStatus
  type: object
- description: ''
  name: IpAddress
  type: object
- description: ''
  name: NtpServerName
  type: object
provider_name: Amazon Panorama
provider_slug: amazon-panorama
schema_file: json-schema/openapi-ntp-status-schema.json
slug: openapi-ntp-status
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-panorama/refs/heads/main/json-schema/openapi-ntp-status-schema.json\",\n  \"title\": \"NtpStatus\",\n  \"description\": \"Details about an NTP server connection.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ConnectionStatus\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NetworkConnectionStatus\"\n        },\n        {\n          \"description\": \"The connection's status.\"\n        }\n      ]\n    },\n    \"IpAddress\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IpAddress\"\n        },\n        {\n          \"description\": \"The IP address of the server.\"\n        }\n      ]\n    },\n    \"NtpServerName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NtpServerName\"\n        },\n        {\n          \"description\": \"The domain\
  \ name of the server.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-panorama/refs/heads/main/json-schema/openapi-ntp-status-schema.json
tags:
- AWS
- Cameras
- Computer Vision
- Edge ML
- Industrial IoT
title: NtpStatus
---
