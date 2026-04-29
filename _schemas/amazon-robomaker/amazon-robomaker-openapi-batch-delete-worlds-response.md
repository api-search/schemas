---
description: BatchDeleteWorldsResponse schema from openapi
layout: schema
name: BatchDeleteWorldsResponse
properties_list:
- description: ''
  name: unprocessedWorlds
  type: object
provider_name: Amazon RoboMaker
provider_slug: amazon-robomaker
schema_file: json-schema/amazon-robomaker-openapi-batch-delete-worlds-response-schema.json
slug: amazon-robomaker-openapi-batch-delete-worlds-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-robomaker/refs/heads/main/json-schema/amazon-robomaker-openapi-batch-delete-worlds-response-schema.json\",\n  \"title\": \"BatchDeleteWorldsResponse\",\n  \"description\": \"BatchDeleteWorldsResponse schema from openapi\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"unprocessedWorlds\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Arns\"\n        },\n        {\n          \"description\": \"A list of unprocessed worlds associated with the call. These worlds were not deleted.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-robomaker/refs/heads/main/json-schema/amazon-robomaker-openapi-batch-delete-worlds-response-schema.json
tags:
- AWS
- Robotics
- Simulation
title: BatchDeleteWorldsResponse
---
