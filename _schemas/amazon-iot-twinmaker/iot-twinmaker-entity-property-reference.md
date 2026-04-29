---
description: An object that uniquely identifies an entity property.
layout: schema
name: EntityPropertyReference
properties_list:
- description: ''
  name: componentName
  type: object
- description: ''
  name: externalIdProperty
  type: object
- description: ''
  name: entityId
  type: object
- description: ''
  name: propertyName
  type: object
provider_name: Amazon IoT TwinMaker
provider_slug: amazon-iot-twinmaker
schema_file: json-schema/iot-twinmaker-entity-property-reference-schema.json
slug: iot-twinmaker-entity-property-reference
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-twinmaker/refs/heads/main/json-schema/iot-twinmaker-entity-property-reference-schema.json\",\n  \"title\": \"EntityPropertyReference\",\n  \"description\": \"An object that uniquely identifies an entity property.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"componentName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Name\"\n        },\n        {\n          \"description\": \"The name of the component.\"\n        }\n      ]\n    },\n    \"externalIdProperty\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ExternalIdProperty\"\n        },\n        {\n          \"description\": \"A mapping of external IDs to property names. External IDs uniquely identify properties from external data stores.\"\n        }\n      ]\n    },\n    \"entityId\": {\n      \"allOf\": [\n\
  \        {\n          \"$ref\": \"#/components/schemas/EntityId\"\n        },\n        {\n          \"description\": \"The ID of the entity.\"\n        }\n      ]\n    },\n    \"propertyName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Name\"\n        },\n        {\n          \"description\": \"The name of the property.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"propertyName\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-twinmaker/refs/heads/main/json-schema/iot-twinmaker-entity-property-reference-schema.json
tags:
- AWS
- 3D Visualization
- Digital Twin
- Industrial IoT
- IoT
title: EntityPropertyReference
---
