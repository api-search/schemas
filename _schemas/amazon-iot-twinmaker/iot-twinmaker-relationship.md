---
description: An object that specifies a relationship with another component type.
layout: schema
name: Relationship
properties_list:
- description: ''
  name: targetComponentTypeId
  type: object
- description: ''
  name: relationshipType
  type: object
provider_name: Amazon IoT TwinMaker
provider_slug: amazon-iot-twinmaker
schema_file: json-schema/iot-twinmaker-relationship-schema.json
slug: iot-twinmaker-relationship
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-twinmaker/refs/heads/main/json-schema/iot-twinmaker-relationship-schema.json\",\n  \"title\": \"Relationship\",\n  \"description\": \"An object that specifies a relationship with another component type.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"targetComponentTypeId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ComponentTypeId\"\n        },\n        {\n          \"description\": \"The ID of the target component type associated with this relationship.\"\n        }\n      ]\n    },\n    \"relationshipType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The type of the relationship.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-twinmaker/refs/heads/main/json-schema/iot-twinmaker-relationship-schema.json
tags:
- AWS
- 3D Visualization
- Digital Twin
- Industrial IoT
- IoT
title: Relationship
---
