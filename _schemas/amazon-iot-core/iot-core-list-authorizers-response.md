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
provider_name: Amazon IoT Core
provider_slug: amazon-iot-core
schema_file: json-schema/iot-core-list-authorizers-response-schema.json
slug: iot-core-list-authorizers-response
source_filename: iot-core-list-authorizers-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-core/refs/heads/main/json-schema/iot-core-list-authorizers-response-schema.json\",\n  \"title\": \"ListAuthorizersResponse\",\n  \"description\": \"ListAuthorizersResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"authorizers\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Authorizers\"\n        },\n        {\n          \"description\": \"The authorizers.\"\n        }\n      ]\n    },\n    \"nextMarker\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Marker\"\n        },\n        {\n          \"description\": \"A marker used to get the next set of results.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-core/refs/heads/main/json-schema/iot-core-list-authorizers-response-schema.json
tags:
- Device Management
- IoT
- MQTT
- Message Routing
title: ListAuthorizersResponse
---
