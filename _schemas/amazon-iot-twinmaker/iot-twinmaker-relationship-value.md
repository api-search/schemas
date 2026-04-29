---
description: A value that associates a component and an entity.
layout: schema
name: RelationshipValue
properties_list:
- description: ''
  name: targetEntityId
  type: object
- description: ''
  name: targetComponentName
  type: object
provider_name: Amazon IoT TwinMaker
provider_slug: amazon-iot-twinmaker
schema_file: json-schema/iot-twinmaker-relationship-value-schema.json
slug: iot-twinmaker-relationship-value
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-twinmaker/refs/heads/main/json-schema/iot-twinmaker-relationship-value-schema.json\",\n  \"title\": \"RelationshipValue\",\n  \"description\": \"A value that associates a component and an entity.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"targetEntityId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EntityId\"\n        },\n        {\n          \"description\": \"The ID of the target entity associated with this relationship value.\"\n        }\n      ]\n    },\n    \"targetComponentName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Name\"\n        },\n        {\n          \"description\": \"The name of the target component associated with the relationship value.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-twinmaker/refs/heads/main/json-schema/iot-twinmaker-relationship-value-schema.json
tags:
- AWS
- 3D Visualization
- Digital Twin
- Industrial IoT
- IoT
title: RelationshipValue
---
