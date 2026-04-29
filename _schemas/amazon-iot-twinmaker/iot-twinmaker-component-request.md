---
description: An object that sets information about a component type create or update request.
layout: schema
name: ComponentRequest
properties_list:
- description: ''
  name: description
  type: object
- description: ''
  name: componentTypeId
  type: object
- description: An object that maps strings to the properties to set in the component type. Each string in the mapping must be unique to this object.
  name: properties
  type: object
- description: ''
  name: propertyGroups
  type: object
provider_name: Amazon IoT TwinMaker
provider_slug: amazon-iot-twinmaker
schema_file: json-schema/iot-twinmaker-component-request-schema.json
slug: iot-twinmaker-component-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-twinmaker/refs/heads/main/json-schema/iot-twinmaker-component-request-schema.json\",\n  \"title\": \"ComponentRequest\",\n  \"description\": \"An object that sets information about a component type create or update request.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"description\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Description\"\n        },\n        {\n          \"description\": \"The description of the component request.\"\n        }\n      ]\n    },\n    \"componentTypeId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ComponentTypeId\"\n        },\n        {\n          \"description\": \"The ID of the component type.\"\n        }\n      ]\n    },\n    \"properties\": {\n      \"description\": \"An object that maps strings to the properties to set\
  \ in the component type. Each string in the mapping must be unique to this object.\"\n    },\n    \"propertyGroups\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ComponentPropertyGroupRequests\"\n        },\n        {\n          \"description\": \"The property groups.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-twinmaker/refs/heads/main/json-schema/iot-twinmaker-component-request-schema.json
tags:
- AWS
- 3D Visualization
- Digital Twin
- Industrial IoT
- IoT
title: ComponentRequest
---
