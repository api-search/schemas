---
description: BatchDeleteWorldsRequest schema from openapi
layout: schema
name: BatchDeleteWorldsRequest
properties_list:
- description: ''
  name: worlds
  type: object
provider_name: Amazon RoboMaker
provider_slug: amazon-robomaker
schema_file: json-schema/amazon-robomaker-openapi-batch-delete-worlds-request-schema.json
slug: amazon-robomaker-openapi-batch-delete-worlds-request
source_filename: amazon-robomaker-openapi-batch-delete-worlds-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-robomaker/refs/heads/main/json-schema/amazon-robomaker-openapi-batch-delete-worlds-request-schema.json\",\n  \"title\": \"BatchDeleteWorldsRequest\",\n  \"description\": \"BatchDeleteWorldsRequest schema from openapi\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"worlds\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Arns\"\n        },\n        {\n          \"description\": \"A list of Amazon Resource Names (arns) that correspond to worlds to delete.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"worlds\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-robomaker/refs/heads/main/json-schema/amazon-robomaker-openapi-batch-delete-worlds-request-schema.json
tags:
- AWS
- Robotics
- Simulation
title: BatchDeleteWorldsRequest
---
