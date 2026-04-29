---
description: The component property group request.
layout: schema
name: ComponentPropertyGroupRequest
properties_list:
- description: ''
  name: groupType
  type: object
- description: ''
  name: propertyNames
  type: object
- description: ''
  name: updateType
  type: object
provider_name: Amazon IoT TwinMaker
provider_slug: amazon-iot-twinmaker
schema_file: json-schema/iot-twinmaker-component-property-group-request-schema.json
slug: iot-twinmaker-component-property-group-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-twinmaker/refs/heads/main/json-schema/iot-twinmaker-component-property-group-request-schema.json\",\n  \"title\": \"ComponentPropertyGroupRequest\",\n  \"description\": \"The component property group request.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"groupType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GroupType\"\n        },\n        {\n          \"description\": \"The group type.\"\n        }\n      ]\n    },\n    \"propertyNames\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PropertyNames\"\n        },\n        {\n          \"description\": \"The property names.\"\n        }\n      ]\n    },\n    \"updateType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PropertyGroupUpdateType\"\n        },\n        {\n          \"\
  description\": \"The update type.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-twinmaker/refs/heads/main/json-schema/iot-twinmaker-component-property-group-request-schema.json
tags:
- AWS
- 3D Visualization
- Digital Twin
- Industrial IoT
- IoT
title: ComponentPropertyGroupRequest
---
