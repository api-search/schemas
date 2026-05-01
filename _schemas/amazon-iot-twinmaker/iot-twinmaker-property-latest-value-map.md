---
description: PropertyLatestValueMap schema
layout: schema
name: PropertyLatestValueMap
properties_list: []
provider_name: Amazon IoT TwinMaker
provider_slug: amazon-iot-twinmaker
schema_file: json-schema/iot-twinmaker-property-latest-value-map-schema.json
slug: iot-twinmaker-property-latest-value-map
source_filename: iot-twinmaker-property-latest-value-map-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-twinmaker/refs/heads/main/json-schema/iot-twinmaker-property-latest-value-map-schema.json\",\n  \"title\": \"PropertyLatestValueMap\",\n  \"description\": \"PropertyLatestValueMap schema\",\n  \"type\": \"object\",\n  \"additionalProperties\": {\n    \"type\": \"object\",\n    \"required\": [\n      \"propertyReference\"\n    ],\n    \"properties\": {\n      \"propertyReference\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/EntityPropertyReference\"\n          },\n          {\n            \"description\": \"An object that specifies information about a property.\"\n          }\n        ]\n      },\n      \"propertyValue\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/DataValue\"\n          },\n          {\n            \"description\": \"The value of the property.\"\
  \n          }\n        ]\n      }\n    },\n    \"description\": \"The latest value of the property.\"\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-twinmaker/refs/heads/main/json-schema/iot-twinmaker-property-latest-value-map-schema.json
tags:
- 3D Visualization
- Digital Twin
- Industrial IoT
- IoT
title: PropertyLatestValueMap
---
