---
description: CreateProjectRequest schema from Amazon CodeCatalyst
layout: schema
name: CreateProjectRequest
properties_list:
- description: ''
  name: displayName
  type: object
- description: ''
  name: description
  type: object
provider_name: Amazon CodeCatalyst
provider_slug: amazon-codecatalyst
schema_file: json-schema/amazon-codecatalyst-create-project-request-schema.json
slug: amazon-codecatalyst-create-project-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codecatalyst/refs/heads/main/json-schema/amazon-codecatalyst-create-project-request-schema.json\",\n  \"title\": \"CreateProjectRequest\",\n  \"description\": \"CreateProjectRequest schema from Amazon CodeCatalyst\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"displayName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ProjectDisplayName\"\n        },\n        {\n          \"description\": \"The friendly name of the project that will be displayed to users.\"\n        }\n      ]\n    },\n    \"description\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ProjectDescription\"\n        },\n        {\n          \"description\": \"The description of the project. This description will be displayed to all users of the project. We recommend providing a brief description of the\
  \ project and its intended purpose.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"displayName\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codecatalyst/refs/heads/main/json-schema/amazon-codecatalyst-create-project-request-schema.json
tags:
- Amazon
- AWS
- Developer Tools
- CI/CD
- Collaboration
- DevOps
- Source Control
title: CreateProjectRequest
---
