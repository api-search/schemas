---
description: GetWorldTemplateBodyRequest schema from openapi
layout: schema
name: GetWorldTemplateBodyRequest
properties_list:
- description: ''
  name: template
  type: object
- description: ''
  name: generationJob
  type: object
provider_name: Amazon RoboMaker
provider_slug: amazon-robomaker
schema_file: json-schema/amazon-robomaker-openapi-get-world-template-body-request-schema.json
slug: amazon-robomaker-openapi-get-world-template-body-request
source_filename: amazon-robomaker-openapi-get-world-template-body-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-robomaker/refs/heads/main/json-schema/amazon-robomaker-openapi-get-world-template-body-request-schema.json\",\n  \"title\": \"GetWorldTemplateBodyRequest\",\n  \"description\": \"GetWorldTemplateBodyRequest schema from openapi\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"template\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Arn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (arn) of the world template.\"\n        }\n      ]\n    },\n    \"generationJob\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Arn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (arn) of the world generator job.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-robomaker/refs/heads/main/json-schema/amazon-robomaker-openapi-get-world-template-body-request-schema.json
tags:
- Robotics
- Simulation
title: GetWorldTemplateBodyRequest
---
