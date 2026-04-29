---
description: The component update request.
layout: schema
name: ComponentUpdateRequest
properties_list:
- description: ''
  name: updateType
  type: object
- description: ''
  name: description
  type: object
- description: ''
  name: componentTypeId
  type: object
- description: ''
  name: propertyUpdates
  type: object
- description: ''
  name: propertyGroupUpdates
  type: object
provider_name: Amazon IoT TwinMaker
provider_slug: amazon-iot-twinmaker
schema_file: json-schema/iot-twinmaker-component-update-request-schema.json
slug: iot-twinmaker-component-update-request
source_filename: iot-twinmaker-component-update-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-twinmaker/refs/heads/main/json-schema/iot-twinmaker-component-update-request-schema.json\",\n  \"title\": \"ComponentUpdateRequest\",\n  \"description\": \"The component update request.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"updateType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ComponentUpdateType\"\n        },\n        {\n          \"description\": \"The update type of the component update request.\"\n        }\n      ]\n    },\n    \"description\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Description\"\n        },\n        {\n          \"description\": \"The description of the component type.\"\n        }\n      ]\n    },\n    \"componentTypeId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ComponentTypeId\"\n \
  \       },\n        {\n          \"description\": \"The ID of the component type.\"\n        }\n      ]\n    },\n    \"propertyUpdates\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PropertyRequests\"\n        },\n        {\n          \"description\": \"An object that maps strings to the properties to set in the component type update. Each string in the mapping must be unique to this object.\"\n        }\n      ]\n    },\n    \"propertyGroupUpdates\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ComponentPropertyGroupRequests\"\n        },\n        {\n          \"description\": \"The property group updates.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-twinmaker/refs/heads/main/json-schema/iot-twinmaker-component-update-request-schema.json
tags:
- AWS
- 3D Visualization
- Digital Twin
- Industrial IoT
- IoT
title: ComponentUpdateRequest
---
