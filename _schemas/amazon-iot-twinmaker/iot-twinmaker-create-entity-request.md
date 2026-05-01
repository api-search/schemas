---
description: CreateEntityRequest schema
layout: schema
name: CreateEntityRequest
properties_list:
- description: ''
  name: entityId
  type: object
- description: ''
  name: entityName
  type: object
- description: ''
  name: description
  type: object
- description: ''
  name: components
  type: object
- description: ''
  name: parentEntityId
  type: object
- description: ''
  name: tags
  type: object
provider_name: Amazon IoT TwinMaker
provider_slug: amazon-iot-twinmaker
schema_file: json-schema/iot-twinmaker-create-entity-request-schema.json
slug: iot-twinmaker-create-entity-request
source_filename: iot-twinmaker-create-entity-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-twinmaker/refs/heads/main/json-schema/iot-twinmaker-create-entity-request-schema.json\",\n  \"title\": \"CreateEntityRequest\",\n  \"description\": \"CreateEntityRequest schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"entityId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EntityId\"\n        },\n        {\n          \"description\": \"The ID of the entity.\"\n        }\n      ]\n    },\n    \"entityName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EntityName\"\n        },\n        {\n          \"description\": \"The name of the entity.\"\n        }\n      ]\n    },\n    \"description\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Description\"\n        },\n        {\n          \"description\": \"The description of the entity.\"\
  \n        }\n      ]\n    },\n    \"components\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ComponentsMapRequest\"\n        },\n        {\n          \"description\": \"An object that maps strings to the components in the entity. Each string in the mapping must be unique to this object.\"\n        }\n      ]\n    },\n    \"parentEntityId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ParentEntityId\"\n        },\n        {\n          \"description\": \"The ID of the entity's parent entity.\"\n        }\n      ]\n    },\n    \"tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TagMap\"\n        },\n        {\n          \"description\": \"Metadata that you can use to manage the entity.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"entityName\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-twinmaker/refs/heads/main/json-schema/iot-twinmaker-create-entity-request-schema.json
tags:
- 3D Visualization
- Digital Twin
- Industrial IoT
- IoT
title: CreateEntityRequest
---
