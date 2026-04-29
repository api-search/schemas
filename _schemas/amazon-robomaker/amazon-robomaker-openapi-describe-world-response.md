---
description: DescribeWorldResponse schema from openapi
layout: schema
name: DescribeWorldResponse
properties_list:
- description: ''
  name: arn
  type: object
- description: ''
  name: generationJob
  type: object
- description: ''
  name: template
  type: object
- description: ''
  name: createdAt
  type: object
- description: ''
  name: tags
  type: object
- description: ''
  name: worldDescriptionBody
  type: object
provider_name: Amazon RoboMaker
provider_slug: amazon-robomaker
schema_file: json-schema/amazon-robomaker-openapi-describe-world-response-schema.json
slug: amazon-robomaker-openapi-describe-world-response
source_filename: amazon-robomaker-openapi-describe-world-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-robomaker/refs/heads/main/json-schema/amazon-robomaker-openapi-describe-world-response-schema.json\",\n  \"title\": \"DescribeWorldResponse\",\n  \"description\": \"DescribeWorldResponse schema from openapi\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"arn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Arn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (arn) of the world.\"\n        }\n      ]\n    },\n    \"generationJob\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Arn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (arn) of the world generation job that generated the world.\"\n        }\n      ]\n    },\n    \"template\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Arn\"\
  \n        },\n        {\n          \"description\": \"The world template.\"\n        }\n      ]\n    },\n    \"createdAt\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CreatedAt\"\n        },\n        {\n          \"description\": \"The time, in milliseconds since the epoch, when the world was created.\"\n        }\n      ]\n    },\n    \"tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TagMap\"\n        },\n        {\n          \"description\": \"A map that contains tag keys and tag values that are attached to the world.\"\n        }\n      ]\n    },\n    \"worldDescriptionBody\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Json\"\n        },\n        {\n          \"description\": \"Returns the JSON formatted string that describes the contents of your world.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-robomaker/refs/heads/main/json-schema/amazon-robomaker-openapi-describe-world-response-schema.json
tags:
- AWS
- Robotics
- Simulation
title: DescribeWorldResponse
---
