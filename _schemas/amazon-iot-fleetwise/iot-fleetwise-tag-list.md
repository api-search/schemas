---
description: TagList schema
layout: schema
name: TagList
properties_list: []
provider_name: Amazon IoT FleetWise
provider_slug: amazon-iot-fleetwise
schema_file: json-schema/iot-fleetwise-tag-list-schema.json
slug: iot-fleetwise-tag-list
source_filename: iot-fleetwise-tag-list-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-fleetwise/refs/heads/main/json-schema/iot-fleetwise-tag-list-schema.json\",\n  \"title\": \"TagList\",\n  \"description\": \"TagList schema\",\n  \"type\": \"array\",\n  \"items\": {\n    \"type\": \"object\",\n    \"required\": [\n      \"Key\",\n      \"Value\"\n    ],\n    \"properties\": {\n      \"Key\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/TagKey\"\n          },\n          {\n            \"description\": \"The tag's key.\"\n          }\n        ]\n      },\n      \"Value\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/TagValue\"\n          },\n          {\n            \"description\": \"The tag's value.\"\n          }\n        ]\n      }\n    },\n    \"description\": \"A set of key/value pairs that are used to manage the resource.\"\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-fleetwise/refs/heads/main/json-schema/iot-fleetwise-tag-list-schema.json
tags:
- Automotive
- Connected Vehicles
- IoT
- Telematics
- Vehicle Data
title: TagList
---
