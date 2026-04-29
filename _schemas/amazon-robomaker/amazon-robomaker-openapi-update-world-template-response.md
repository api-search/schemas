---
description: UpdateWorldTemplateResponse schema from openapi
layout: schema
name: UpdateWorldTemplateResponse
properties_list:
- description: ''
  name: arn
  type: object
- description: ''
  name: name
  type: object
- description: ''
  name: createdAt
  type: object
- description: ''
  name: lastUpdatedAt
  type: object
provider_name: Amazon RoboMaker
provider_slug: amazon-robomaker
schema_file: json-schema/amazon-robomaker-openapi-update-world-template-response-schema.json
slug: amazon-robomaker-openapi-update-world-template-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-robomaker/refs/heads/main/json-schema/amazon-robomaker-openapi-update-world-template-response-schema.json\",\n  \"title\": \"UpdateWorldTemplateResponse\",\n  \"description\": \"UpdateWorldTemplateResponse schema from openapi\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"arn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Arn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (arn) of the world template.\"\n        }\n      ]\n    },\n    \"name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TemplateName\"\n        },\n        {\n          \"description\": \"The name of the world template.\"\n        }\n      ]\n    },\n    \"createdAt\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CreatedAt\"\n        },\n\
  \        {\n          \"description\": \"The time, in milliseconds since the epoch, when the world template was created.\"\n        }\n      ]\n    },\n    \"lastUpdatedAt\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LastUpdatedAt\"\n        },\n        {\n          \"description\": \"The time, in milliseconds since the epoch, when the world template was last updated.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-robomaker/refs/heads/main/json-schema/amazon-robomaker-openapi-update-world-template-response-schema.json
tags:
- AWS
- Robotics
- Simulation
title: UpdateWorldTemplateResponse
---
