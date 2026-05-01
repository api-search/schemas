---
description: CreateProjectResponse schema from Amazon CodeCatalyst
layout: schema
name: CreateProjectResponse
properties_list:
- description: ''
  name: spaceName
  type: object
- description: ''
  name: name
  type: object
- description: ''
  name: displayName
  type: object
- description: ''
  name: description
  type: object
provider_name: Amazon CodeCatalyst
provider_slug: amazon-codecatalyst
schema_file: json-schema/amazon-codecatalyst-create-project-response-schema.json
slug: amazon-codecatalyst-create-project-response
source_filename: amazon-codecatalyst-create-project-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codecatalyst/refs/heads/main/json-schema/amazon-codecatalyst-create-project-response-schema.json\",\n  \"title\": \"CreateProjectResponse\",\n  \"description\": \"CreateProjectResponse schema from Amazon CodeCatalyst\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"spaceName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NameString\"\n        },\n        {\n          \"description\": \"The name of the space.\"\n        }\n      ]\n    },\n    \"name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NameString\"\n        },\n        {\n          \"description\": \"The name of the project in the space.\"\n        }\n      ]\n    },\n    \"displayName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n         \
  \ \"description\": \"The friendly name of the project.\"\n        }\n      ]\n    },\n    \"description\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The description of the project.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"name\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codecatalyst/refs/heads/main/json-schema/amazon-codecatalyst-create-project-response-schema.json
tags:
- Amazon
- Developer Tools
- CI/CD
- Collaboration
- DevOps
- Source Control
title: CreateProjectResponse
---
