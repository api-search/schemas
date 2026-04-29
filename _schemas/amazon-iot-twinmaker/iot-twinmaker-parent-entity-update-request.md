---
description: The parent entity update request.
layout: schema
name: ParentEntityUpdateRequest
properties_list:
- description: ''
  name: updateType
  type: object
- description: ''
  name: parentEntityId
  type: object
provider_name: Amazon IoT TwinMaker
provider_slug: amazon-iot-twinmaker
schema_file: json-schema/iot-twinmaker-parent-entity-update-request-schema.json
slug: iot-twinmaker-parent-entity-update-request
source_filename: iot-twinmaker-parent-entity-update-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-twinmaker/refs/heads/main/json-schema/iot-twinmaker-parent-entity-update-request-schema.json\",\n  \"title\": \"ParentEntityUpdateRequest\",\n  \"description\": \"The parent entity update request.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"updateType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ParentEntityUpdateType\"\n        },\n        {\n          \"description\": \"The type of the update.\"\n        }\n      ]\n    },\n    \"parentEntityId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ParentEntityId\"\n        },\n        {\n          \"description\": \"The ID of the parent entity.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"updateType\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-twinmaker/refs/heads/main/json-schema/iot-twinmaker-parent-entity-update-request-schema.json
tags:
- AWS
- 3D Visualization
- Digital Twin
- Industrial IoT
- IoT
title: ParentEntityUpdateRequest
---
