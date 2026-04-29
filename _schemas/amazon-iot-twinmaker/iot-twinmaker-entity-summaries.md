---
description: EntitySummaries schema
layout: schema
name: EntitySummaries
properties_list: []
provider_name: Amazon IoT TwinMaker
provider_slug: amazon-iot-twinmaker
schema_file: json-schema/iot-twinmaker-entity-summaries-schema.json
slug: iot-twinmaker-entity-summaries
source_filename: iot-twinmaker-entity-summaries-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-twinmaker/refs/heads/main/json-schema/iot-twinmaker-entity-summaries-schema.json\",\n  \"title\": \"EntitySummaries\",\n  \"description\": \"EntitySummaries schema\",\n  \"type\": \"array\",\n  \"items\": {\n    \"type\": \"object\",\n    \"required\": [\n      \"entityId\",\n      \"entityName\",\n      \"arn\",\n      \"status\",\n      \"creationDateTime\",\n      \"updateDateTime\"\n    ],\n    \"properties\": {\n      \"entityId\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/EntityId\"\n          },\n          {\n            \"description\": \"The ID of the entity.\"\n          }\n        ]\n      },\n      \"entityName\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/EntityName\"\n          },\n          {\n            \"description\": \"The name of the\
  \ entity.\"\n          }\n        ]\n      },\n      \"arn\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/TwinMakerArn\"\n          },\n          {\n            \"description\": \"The ARN of the entity.\"\n          }\n        ]\n      },\n      \"parentEntityId\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/ParentEntityId\"\n          },\n          {\n            \"description\": \"The ID of the parent entity.\"\n          }\n        ]\n      },\n      \"status\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/Status\"\n          },\n          {\n            \"description\": \"The current status of the entity.\"\n          }\n        ]\n      },\n      \"description\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/Description\"\n          },\n          {\n            \"description\": \"The description of the entity.\"\n          }\n   \
  \     ]\n      },\n      \"hasChildEntities\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/Boolean\"\n          },\n          {\n            \"description\": \"A Boolean value that specifies whether the entity has child entities or not.\"\n          }\n        ]\n      },\n      \"creationDateTime\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/Timestamp\"\n          },\n          {\n            \"description\": \"The date and time when the entity was created.\"\n          }\n        ]\n      },\n      \"updateDateTime\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/Timestamp\"\n          },\n          {\n            \"description\": \"The last date and time when the entity was updated.\"\n          }\n        ]\n      }\n    },\n    \"description\": \"An object that contains information about an entity.\"\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-twinmaker/refs/heads/main/json-schema/iot-twinmaker-entity-summaries-schema.json
tags:
- AWS
- 3D Visualization
- Digital Twin
- Industrial IoT
- IoT
title: EntitySummaries
---
