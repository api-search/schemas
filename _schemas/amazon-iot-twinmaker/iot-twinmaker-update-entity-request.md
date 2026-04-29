---
description: UpdateEntityRequest schema
layout: schema
name: UpdateEntityRequest
properties_list:
- description: ''
  name: entityName
  type: object
- description: ''
  name: description
  type: object
- description: ''
  name: componentUpdates
  type: object
- description: ''
  name: parentEntityUpdate
  type: object
provider_name: Amazon IoT TwinMaker
provider_slug: amazon-iot-twinmaker
schema_file: json-schema/iot-twinmaker-update-entity-request-schema.json
slug: iot-twinmaker-update-entity-request
source_filename: iot-twinmaker-update-entity-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-twinmaker/refs/heads/main/json-schema/iot-twinmaker-update-entity-request-schema.json\",\n  \"title\": \"UpdateEntityRequest\",\n  \"description\": \"UpdateEntityRequest schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"entityName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EntityName\"\n        },\n        {\n          \"description\": \"The name of the entity.\"\n        }\n      ]\n    },\n    \"description\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Description\"\n        },\n        {\n          \"description\": \"The description of the entity.\"\n        }\n      ]\n    },\n    \"componentUpdates\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ComponentUpdatesMapRequest\"\n        },\n        {\n          \"description\"\
  : \"An object that maps strings to the component updates in the request. Each string in the mapping must be unique to this object.\"\n        }\n      ]\n    },\n    \"parentEntityUpdate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ParentEntityUpdateRequest\"\n        },\n        {\n          \"description\": \"An object that describes the update request for a parent entity.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-twinmaker/refs/heads/main/json-schema/iot-twinmaker-update-entity-request-schema.json
tags:
- AWS
- 3D Visualization
- Digital Twin
- Industrial IoT
- IoT
title: UpdateEntityRequest
---
