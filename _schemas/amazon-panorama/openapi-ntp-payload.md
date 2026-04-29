---
description: Network time protocol (NTP) server settings. Use this option to connect to local NTP servers instead of <code>pool.ntp.org</code>.
layout: schema
name: NtpPayload
properties_list:
- description: ''
  name: NtpServers
  type: object
provider_name: Amazon Panorama
provider_slug: amazon-panorama
schema_file: json-schema/openapi-ntp-payload-schema.json
slug: openapi-ntp-payload
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-panorama/refs/heads/main/json-schema/openapi-ntp-payload-schema.json\",\n  \"title\": \"NtpPayload\",\n  \"description\": \"Network time protocol (NTP) server settings. Use this option to connect to local NTP servers instead of <code>pool.ntp.org</code>.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"NtpServers\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NtpServerList\"\n        },\n        {\n          \"description\": \"NTP servers to use, in order of preference.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"NtpServers\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-panorama/refs/heads/main/json-schema/openapi-ntp-payload-schema.json
tags:
- AWS
- Cameras
- Computer Vision
- Edge ML
- Industrial IoT
title: NtpPayload
---
