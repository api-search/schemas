---
description: ListAttachedPoliciesResponse schema
layout: schema
name: ListAttachedPoliciesResponse
properties_list:
- description: ''
  name: policies
  type: object
- description: ''
  name: nextMarker
  type: object
provider_name: Amazon IoT Core
provider_slug: amazon-iot-core
schema_file: json-schema/iot-core-list-attached-policies-response-schema.json
slug: iot-core-list-attached-policies-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-core/refs/heads/main/json-schema/iot-core-list-attached-policies-response-schema.json\",\n  \"title\": \"ListAttachedPoliciesResponse\",\n  \"description\": \"ListAttachedPoliciesResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"policies\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Policies\"\n        },\n        {\n          \"description\": \"The policies.\"\n        }\n      ]\n    },\n    \"nextMarker\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Marker\"\n        },\n        {\n          \"description\": \"The token to retrieve the next set of results, or ``null`` if there are no more results.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-core/refs/heads/main/json-schema/iot-core-list-attached-policies-response-schema.json
tags:
- AWS
- Device Management
- IoT
- MQTT
- Message Routing
title: ListAttachedPoliciesResponse
---
