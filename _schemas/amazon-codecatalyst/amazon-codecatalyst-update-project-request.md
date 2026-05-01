---
description: UpdateProjectRequest schema from Amazon CodeCatalyst
layout: schema
name: UpdateProjectRequest
properties_list:
- description: ''
  name: description
  type: object
provider_name: Amazon CodeCatalyst
provider_slug: amazon-codecatalyst
schema_file: json-schema/amazon-codecatalyst-update-project-request-schema.json
slug: amazon-codecatalyst-update-project-request
source_filename: amazon-codecatalyst-update-project-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codecatalyst/refs/heads/main/json-schema/amazon-codecatalyst-update-project-request-schema.json\",\n  \"title\": \"UpdateProjectRequest\",\n  \"description\": \"UpdateProjectRequest schema from Amazon CodeCatalyst\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"description\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ProjectDescription\"\n        },\n        {\n          \"description\": \"The description of the project.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codecatalyst/refs/heads/main/json-schema/amazon-codecatalyst-update-project-request-schema.json
tags:
- Amazon
- Developer Tools
- CI/CD
- Collaboration
- DevOps
- Source Control
title: UpdateProjectRequest
---
