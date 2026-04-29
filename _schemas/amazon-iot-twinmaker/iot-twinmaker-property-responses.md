---
description: PropertyResponses schema
layout: schema
name: PropertyResponses
properties_list: []
provider_name: Amazon IoT TwinMaker
provider_slug: amazon-iot-twinmaker
schema_file: json-schema/iot-twinmaker-property-responses-schema.json
slug: iot-twinmaker-property-responses
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-twinmaker/refs/heads/main/json-schema/iot-twinmaker-property-responses-schema.json\",\n  \"title\": \"PropertyResponses\",\n  \"description\": \"PropertyResponses schema\",\n  \"type\": \"object\",\n  \"additionalProperties\": {\n    \"type\": \"object\",\n    \"properties\": {\n      \"definition\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/PropertyDefinitionResponse\"\n          },\n          {\n            \"description\": \"An object that specifies information about a property.\"\n          }\n        ]\n      },\n      \"value\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/DataValue\"\n          },\n          {\n            \"description\": \"The value of the property.\"\n          }\n        ]\n      }\n    },\n    \"description\": \"An object that contains\
  \ information about a property response.\"\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-twinmaker/refs/heads/main/json-schema/iot-twinmaker-property-responses-schema.json
tags:
- AWS
- 3D Visualization
- Digital Twin
- Industrial IoT
- IoT
title: PropertyResponses
---
