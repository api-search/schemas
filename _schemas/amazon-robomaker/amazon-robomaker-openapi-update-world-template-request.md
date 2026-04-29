---
description: UpdateWorldTemplateRequest schema from openapi
layout: schema
name: UpdateWorldTemplateRequest
properties_list:
- description: ''
  name: template
  type: object
- description: ''
  name: name
  type: object
- description: ''
  name: templateBody
  type: object
- description: ''
  name: templateLocation
  type: object
provider_name: Amazon RoboMaker
provider_slug: amazon-robomaker
schema_file: json-schema/amazon-robomaker-openapi-update-world-template-request-schema.json
slug: amazon-robomaker-openapi-update-world-template-request
source_filename: amazon-robomaker-openapi-update-world-template-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-robomaker/refs/heads/main/json-schema/amazon-robomaker-openapi-update-world-template-request-schema.json\",\n  \"title\": \"UpdateWorldTemplateRequest\",\n  \"description\": \"UpdateWorldTemplateRequest schema from openapi\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"template\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Arn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (arn) of the world template to update.\"\n        }\n      ]\n    },\n    \"name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TemplateName\"\n        },\n        {\n          \"description\": \"The name of the template.\"\n        }\n      ]\n    },\n    \"templateBody\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Json\"\n    \
  \    },\n        {\n          \"description\": \"The world template body.\"\n        }\n      ]\n    },\n    \"templateLocation\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TemplateLocation\"\n        },\n        {\n          \"description\": \"The location of the world template.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"template\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-robomaker/refs/heads/main/json-schema/amazon-robomaker-openapi-update-world-template-request-schema.json
tags:
- AWS
- Robotics
- Simulation
title: UpdateWorldTemplateRequest
---
