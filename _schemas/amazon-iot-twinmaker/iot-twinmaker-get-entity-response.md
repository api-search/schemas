---
description: GetEntityResponse schema
layout: schema
name: GetEntityResponse
properties_list:
- description: ''
  name: entityId
  type: object
- description: ''
  name: entityName
  type: object
- description: ''
  name: arn
  type: object
- description: ''
  name: status
  type: object
- description: ''
  name: workspaceId
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
  name: hasChildEntities
  type: object
- description: ''
  name: creationDateTime
  type: object
- description: ''
  name: updateDateTime
  type: object
- description: ''
  name: syncSource
  type: object
provider_name: Amazon IoT TwinMaker
provider_slug: amazon-iot-twinmaker
schema_file: json-schema/iot-twinmaker-get-entity-response-schema.json
slug: iot-twinmaker-get-entity-response
source_filename: iot-twinmaker-get-entity-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-twinmaker/refs/heads/main/json-schema/iot-twinmaker-get-entity-response-schema.json\",\n  \"title\": \"GetEntityResponse\",\n  \"description\": \"GetEntityResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"entityId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EntityId\"\n        },\n        {\n          \"description\": \"The ID of the entity.\"\n        }\n      ]\n    },\n    \"entityName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EntityName\"\n        },\n        {\n          \"description\": \"The name of the entity.\"\n        }\n      ]\n    },\n    \"arn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TwinMakerArn\"\n        },\n        {\n          \"description\": \"The ARN of the entity.\"\n        }\n\
  \      ]\n    },\n    \"status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Status\"\n        },\n        {\n          \"description\": \"The current status of the entity.\"\n        }\n      ]\n    },\n    \"workspaceId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Id\"\n        },\n        {\n          \"description\": \"The ID of the workspace.\"\n        }\n      ]\n    },\n    \"description\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Description\"\n        },\n        {\n          \"description\": \"The description of the entity.\"\n        }\n      ]\n    },\n    \"components\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ComponentsMap\"\n        },\n        {\n          \"description\": \"An object that maps strings to the components in the entity. Each string in the mapping must be unique to this object.\"\n        }\n      ]\n    },\n    \"\
  parentEntityId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ParentEntityId\"\n        },\n        {\n          \"description\": \"The ID of the parent entity for this entity.\"\n        }\n      ]\n    },\n    \"hasChildEntities\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Boolean\"\n        },\n        {\n          \"description\": \"A Boolean value that specifies whether the entity has associated child entities.\"\n        }\n      ]\n    },\n    \"creationDateTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The date and time when the entity was created.\"\n        }\n      ]\n    },\n    \"updateDateTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The date and time when the entity was last updated.\"\n        }\n  \
  \    ]\n    },\n    \"syncSource\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SyncSource\"\n        },\n        {\n          \"description\": \"The syncSource of the sync job, if this entity was created by a sync job.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"entityId\",\n    \"entityName\",\n    \"arn\",\n    \"status\",\n    \"workspaceId\",\n    \"parentEntityId\",\n    \"hasChildEntities\",\n    \"creationDateTime\",\n    \"updateDateTime\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-twinmaker/refs/heads/main/json-schema/iot-twinmaker-get-entity-response-schema.json
tags:
- 3D Visualization
- Digital Twin
- Industrial IoT
- IoT
title: GetEntityResponse
---
