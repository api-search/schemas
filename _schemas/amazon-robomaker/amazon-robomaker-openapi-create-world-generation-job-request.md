---
description: CreateWorldGenerationJobRequest schema from openapi
layout: schema
name: CreateWorldGenerationJobRequest
properties_list:
- description: ''
  name: clientRequestToken
  type: object
- description: ''
  name: template
  type: object
- description: ''
  name: worldCount
  type: object
- description: ''
  name: tags
  type: object
- description: ''
  name: worldTags
  type: object
provider_name: Amazon RoboMaker
provider_slug: amazon-robomaker
schema_file: json-schema/amazon-robomaker-openapi-create-world-generation-job-request-schema.json
slug: amazon-robomaker-openapi-create-world-generation-job-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-robomaker/refs/heads/main/json-schema/amazon-robomaker-openapi-create-world-generation-job-request-schema.json\",\n  \"title\": \"CreateWorldGenerationJobRequest\",\n  \"description\": \"CreateWorldGenerationJobRequest schema from openapi\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"clientRequestToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ClientRequestToken\"\n        },\n        {\n          \"description\": \"Unique, case-sensitive identifier that you provide to ensure the idempotency of the request.\"\n        }\n      ]\n    },\n    \"template\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Arn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (arn) of the world template describing the worlds you want to create.\"\n     \
  \   }\n      ]\n    },\n    \"worldCount\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WorldCount\"\n        },\n        {\n          \"description\": \"Information about the world count.\"\n        }\n      ]\n    },\n    \"tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TagMap\"\n        },\n        {\n          \"description\": \"A map that contains tag keys and tag values that are attached to the world generator job.\"\n        }\n      ]\n    },\n    \"worldTags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TagMap\"\n        },\n        {\n          \"description\": \"A map that contains tag keys and tag values that are attached to the generated worlds.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"template\",\n    \"worldCount\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-robomaker/refs/heads/main/json-schema/amazon-robomaker-openapi-create-world-generation-job-request-schema.json
tags:
- AWS
- Robotics
- Simulation
title: CreateWorldGenerationJobRequest
---
