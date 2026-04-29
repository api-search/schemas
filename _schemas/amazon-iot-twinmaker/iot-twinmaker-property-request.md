---
description: An object that sets information about a property.
layout: schema
name: PropertyRequest
properties_list:
- description: ''
  name: definition
  type: object
- description: ''
  name: value
  type: object
- description: ''
  name: updateType
  type: object
provider_name: Amazon IoT TwinMaker
provider_slug: amazon-iot-twinmaker
schema_file: json-schema/iot-twinmaker-property-request-schema.json
slug: iot-twinmaker-property-request
source_filename: iot-twinmaker-property-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-twinmaker/refs/heads/main/json-schema/iot-twinmaker-property-request-schema.json\",\n  \"title\": \"PropertyRequest\",\n  \"description\": \"An object that sets information about a property.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"definition\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PropertyDefinitionRequest\"\n        },\n        {\n          \"description\": \"An object that specifies information about a property.\"\n        }\n      ]\n    },\n    \"value\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DataValue\"\n        },\n        {\n          \"description\": \"The value of the property.\"\n        }\n      ]\n    },\n    \"updateType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PropertyUpdateType\"\n      \
  \  },\n        {\n          \"description\": \"The update type of the update property request.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-twinmaker/refs/heads/main/json-schema/iot-twinmaker-property-request-schema.json
tags:
- AWS
- 3D Visualization
- Digital Twin
- Industrial IoT
- IoT
title: PropertyRequest
---
