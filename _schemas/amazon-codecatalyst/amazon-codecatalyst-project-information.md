---
description: Information about a project in a space.
layout: schema
name: ProjectInformation
properties_list:
- description: ''
  name: name
  type: object
- description: ''
  name: projectId
  type: object
provider_name: Amazon CodeCatalyst
provider_slug: amazon-codecatalyst
schema_file: json-schema/amazon-codecatalyst-project-information-schema.json
slug: amazon-codecatalyst-project-information
source_filename: amazon-codecatalyst-project-information-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codecatalyst/refs/heads/main/json-schema/amazon-codecatalyst-project-information-schema.json\",\n  \"title\": \"ProjectInformation\",\n  \"description\": \"Information about a project in a space.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The name of the project in the space.\"\n        }\n      ]\n    },\n    \"projectId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The system-generated unique ID of the project.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codecatalyst/refs/heads/main/json-schema/amazon-codecatalyst-project-information-schema.json
tags:
- Amazon
- Developer Tools
- CI/CD
- Collaboration
- DevOps
- Source Control
title: ProjectInformation
---
