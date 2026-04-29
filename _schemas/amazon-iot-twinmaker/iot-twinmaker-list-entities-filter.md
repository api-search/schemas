---
description: An object that filters items in a list of entities.
layout: schema
name: ListEntitiesFilter
properties_list:
- description: ''
  name: parentEntityId
  type: object
- description: ''
  name: componentTypeId
  type: object
- description: ''
  name: externalId
  type: object
provider_name: Amazon IoT TwinMaker
provider_slug: amazon-iot-twinmaker
schema_file: json-schema/iot-twinmaker-list-entities-filter-schema.json
slug: iot-twinmaker-list-entities-filter
source_filename: iot-twinmaker-list-entities-filter-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-twinmaker/refs/heads/main/json-schema/iot-twinmaker-list-entities-filter-schema.json\",\n  \"title\": \"ListEntitiesFilter\",\n  \"description\": \"An object that filters items in a list of entities.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"parentEntityId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ParentEntityId\"\n        },\n        {\n          \"description\": \"The parent of the entities in the list.\"\n        }\n      ]\n    },\n    \"componentTypeId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ComponentTypeId\"\n        },\n        {\n          \"description\": \"The ID of the component type in the entities in the list.\"\n        }\n      ]\n    },\n    \"externalId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\
  \n        },\n        {\n          \"description\": \"The external-Id property of a component. The external-Id property is the primary key of an external storage system.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-twinmaker/refs/heads/main/json-schema/iot-twinmaker-list-entities-filter-schema.json
tags:
- AWS
- 3D Visualization
- Digital Twin
- Industrial IoT
- IoT
title: ListEntitiesFilter
---
