---
description: Tags schema
layout: schema
name: Tags
properties_list: []
provider_name: Amazon IoT Events
provider_slug: amazon-iot-events
schema_file: json-schema/iot-events-tags-schema.json
slug: iot-events-tags
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-events/refs/heads/main/json-schema/iot-events-tags-schema.json\",\n  \"title\": \"Tags\",\n  \"description\": \"Tags schema\",\n  \"type\": \"array\",\n  \"items\": {\n    \"type\": \"object\",\n    \"required\": [\n      \"key\",\n      \"value\"\n    ],\n    \"properties\": {\n      \"key\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/TagKey\"\n          },\n          {\n            \"description\": \"The tag's key.\"\n          }\n        ]\n      },\n      \"value\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/TagValue\"\n          },\n          {\n            \"description\": \"The tag's value.\"\n          }\n        ]\n      }\n    },\n    \"description\": \"Metadata that can be used to manage the resource.\"\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-events/refs/heads/main/json-schema/iot-events-tags-schema.json
tags:
- AWS
- Event Detection
- IoT
- State Machine
- Automation
title: Tags
---
