---
description: An object that contains information about a property response.
layout: schema
name: PropertyResponse
properties_list:
- description: ''
  name: definition
  type: object
- description: ''
  name: value
  type: object
provider_name: Amazon IoT TwinMaker
provider_slug: amazon-iot-twinmaker
schema_file: json-schema/iot-twinmaker-property-response-schema.json
slug: iot-twinmaker-property-response
source_filename: iot-twinmaker-property-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-twinmaker/refs/heads/main/json-schema/iot-twinmaker-property-response-schema.json\",\n  \"title\": \"PropertyResponse\",\n  \"description\": \"An object that contains information about a property response.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"definition\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PropertyDefinitionResponse\"\n        },\n        {\n          \"description\": \"An object that specifies information about a property.\"\n        }\n      ]\n    },\n    \"value\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DataValue\"\n        },\n        {\n          \"description\": \"The value of the property.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-twinmaker/refs/heads/main/json-schema/iot-twinmaker-property-response-schema.json
tags:
- 3D Visualization
- Digital Twin
- Industrial IoT
- IoT
title: PropertyResponse
---
