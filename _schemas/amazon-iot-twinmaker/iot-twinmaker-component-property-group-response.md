---
description: The component property group response.
layout: schema
name: ComponentPropertyGroupResponse
properties_list:
- description: ''
  name: groupType
  type: object
- description: ''
  name: propertyNames
  type: object
- description: ''
  name: isInherited
  type: object
provider_name: Amazon IoT TwinMaker
provider_slug: amazon-iot-twinmaker
schema_file: json-schema/iot-twinmaker-component-property-group-response-schema.json
slug: iot-twinmaker-component-property-group-response
source_filename: iot-twinmaker-component-property-group-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-twinmaker/refs/heads/main/json-schema/iot-twinmaker-component-property-group-response-schema.json\",\n  \"title\": \"ComponentPropertyGroupResponse\",\n  \"description\": \"The component property group response.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"groupType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GroupType\"\n        },\n        {\n          \"description\": \"The group type.\"\n        }\n      ]\n    },\n    \"propertyNames\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PropertyNames\"\n        },\n        {\n          \"description\": \"The names of properties\"\n        }\n      ]\n    },\n    \"isInherited\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Boolean\"\n        },\n        {\n          \"description\"\
  : \"A Boolean value that specifies whether the property group is inherited from a parent entity\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"groupType\",\n    \"propertyNames\",\n    \"isInherited\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-twinmaker/refs/heads/main/json-schema/iot-twinmaker-component-property-group-response-schema.json
tags:
- 3D Visualization
- Digital Twin
- Industrial IoT
- IoT
title: ComponentPropertyGroupResponse
---
