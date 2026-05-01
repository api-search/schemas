---
description: CreateWorldTemplateRequest schema from openapi
layout: schema
name: CreateWorldTemplateRequest
properties_list:
- description: ''
  name: clientRequestToken
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
- description: ''
  name: tags
  type: object
provider_name: Amazon RoboMaker
provider_slug: amazon-robomaker
schema_file: json-schema/amazon-robomaker-openapi-create-world-template-request-schema.json
slug: amazon-robomaker-openapi-create-world-template-request
source_filename: amazon-robomaker-openapi-create-world-template-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-robomaker/refs/heads/main/json-schema/amazon-robomaker-openapi-create-world-template-request-schema.json\",\n  \"title\": \"CreateWorldTemplateRequest\",\n  \"description\": \"CreateWorldTemplateRequest schema from openapi\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"clientRequestToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ClientRequestToken\"\n        },\n        {\n          \"description\": \"Unique, case-sensitive identifier that you provide to ensure the idempotency of the request.\"\n        }\n      ]\n    },\n    \"name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TemplateName\"\n        },\n        {\n          \"description\": \"The name of the world template.\"\n        }\n      ]\n    },\n    \"templateBody\": {\n      \"allOf\": [\n      \
  \  {\n          \"$ref\": \"#/components/schemas/Json\"\n        },\n        {\n          \"description\": \"The world template body.\"\n        }\n      ]\n    },\n    \"templateLocation\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TemplateLocation\"\n        },\n        {\n          \"description\": \"The location of the world template.\"\n        }\n      ]\n    },\n    \"tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TagMap\"\n        },\n        {\n          \"description\": \"A map that contains tag keys and tag values that are attached to the world template.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-robomaker/refs/heads/main/json-schema/amazon-robomaker-openapi-create-world-template-request-schema.json
tags:
- Robotics
- Simulation
title: CreateWorldTemplateRequest
---
