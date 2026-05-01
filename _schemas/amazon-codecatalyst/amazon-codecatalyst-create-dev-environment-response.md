---
description: CreateDevEnvironmentResponse schema from Amazon CodeCatalyst
layout: schema
name: CreateDevEnvironmentResponse
properties_list:
- description: ''
  name: spaceName
  type: object
- description: ''
  name: projectName
  type: object
- description: ''
  name: id
  type: object
provider_name: Amazon CodeCatalyst
provider_slug: amazon-codecatalyst
schema_file: json-schema/amazon-codecatalyst-create-dev-environment-response-schema.json
slug: amazon-codecatalyst-create-dev-environment-response
source_filename: amazon-codecatalyst-create-dev-environment-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codecatalyst/refs/heads/main/json-schema/amazon-codecatalyst-create-dev-environment-response-schema.json\",\n  \"title\": \"CreateDevEnvironmentResponse\",\n  \"description\": \"CreateDevEnvironmentResponse schema from Amazon CodeCatalyst\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"spaceName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NameString\"\n        },\n        {\n          \"description\": \"The name of the space.\"\n        }\n      ]\n    },\n    \"projectName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NameString\"\n        },\n        {\n          \"description\": \"The name of the project in the space.\"\n        }\n      ]\n    },\n    \"id\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Uuid\"\n        },\n  \
  \      {\n          \"description\": \"The system-generated unique ID of the Dev Environment. \"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"spaceName\",\n    \"projectName\",\n    \"id\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codecatalyst/refs/heads/main/json-schema/amazon-codecatalyst-create-dev-environment-response-schema.json
tags:
- Amazon
- Developer Tools
- CI/CD
- Collaboration
- DevOps
- Source Control
title: CreateDevEnvironmentResponse
---
