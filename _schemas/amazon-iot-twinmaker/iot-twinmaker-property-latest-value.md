---
description: The latest value of the property.
layout: schema
name: PropertyLatestValue
properties_list:
- description: ''
  name: propertyReference
  type: object
- description: ''
  name: propertyValue
  type: object
provider_name: Amazon IoT TwinMaker
provider_slug: amazon-iot-twinmaker
schema_file: json-schema/iot-twinmaker-property-latest-value-schema.json
slug: iot-twinmaker-property-latest-value
source_filename: iot-twinmaker-property-latest-value-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-twinmaker/refs/heads/main/json-schema/iot-twinmaker-property-latest-value-schema.json\",\n  \"title\": \"PropertyLatestValue\",\n  \"description\": \"The latest value of the property.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"propertyReference\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EntityPropertyReference\"\n        },\n        {\n          \"description\": \"An object that specifies information about a property.\"\n        }\n      ]\n    },\n    \"propertyValue\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DataValue\"\n        },\n        {\n          \"description\": \"The value of the property.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"propertyReference\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-twinmaker/refs/heads/main/json-schema/iot-twinmaker-property-latest-value-schema.json
tags:
- 3D Visualization
- Digital Twin
- Industrial IoT
- IoT
title: PropertyLatestValue
---
