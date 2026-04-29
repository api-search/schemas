---
description: ListAuthorizersResponse schema
layout: schema
name: ListAuthorizersResponse
properties_list:
- description: ''
  name: authorizers
  type: object
- description: ''
  name: nextMarker
  type: object
provider_name: Amazon IoT Device Defender
provider_slug: amazon-iot-device-defender
schema_file: json-schema/iot-device-defender-list-authorizers-response-schema.json
slug: iot-device-defender-list-authorizers-response
source_filename: iot-device-defender-list-authorizers-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-device-defender/refs/heads/main/json-schema/iot-device-defender-list-authorizers-response-schema.json\",\n  \"title\": \"ListAuthorizersResponse\",\n  \"description\": \"ListAuthorizersResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"authorizers\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Authorizers\"\n        },\n        {\n          \"description\": \"The authorizers.\"\n        }\n      ]\n    },\n    \"nextMarker\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Marker\"\n        },\n        {\n          \"description\": \"A marker used to get the next set of results.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-device-defender/refs/heads/main/json-schema/iot-device-defender-list-authorizers-response-schema.json
tags:
- AWS
- Compliance
- IoT
- Security
- Vulnerability Management
title: ListAuthorizersResponse
---
