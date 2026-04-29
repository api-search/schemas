---
description: ListEntitiesResponse schema
layout: schema
name: ListEntitiesResponse
properties_list:
- description: ''
  name: entitySummaries
  type: object
- description: ''
  name: nextToken
  type: object
provider_name: Amazon IoT TwinMaker
provider_slug: amazon-iot-twinmaker
schema_file: json-schema/iot-twinmaker-list-entities-response-schema.json
slug: iot-twinmaker-list-entities-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-twinmaker/refs/heads/main/json-schema/iot-twinmaker-list-entities-response-schema.json\",\n  \"title\": \"ListEntitiesResponse\",\n  \"description\": \"ListEntitiesResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"entitySummaries\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EntitySummaries\"\n        },\n        {\n          \"description\": \"A list of objects that contain information about the entities.\"\n        }\n      ]\n    },\n    \"nextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NextToken\"\n        },\n        {\n          \"description\": \"The string that specifies the next page of results.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-twinmaker/refs/heads/main/json-schema/iot-twinmaker-list-entities-response-schema.json
tags:
- AWS
- 3D Visualization
- Digital Twin
- Industrial IoT
- IoT
title: ListEntitiesResponse
---
