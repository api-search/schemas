---
description: TagProjectRequest schema from AWS CodeStar API
layout: schema
name: TagProjectRequest
properties_list:
- description: ''
  name: id
  type: object
- description: ''
  name: tags
  type: object
provider_name: Amazon CodeStar
provider_slug: amazon-codestar
schema_file: json-schema/codestar-tag-project-request-schema.json
slug: codestar-tag-project-request
source_filename: codestar-tag-project-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codestar/refs/heads/main/json-schema/codestar-tag-project-request-schema.json\",\n  \"title\": \"TagProjectRequest\",\n  \"description\": \"TagProjectRequest schema from AWS CodeStar API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ProjectId\"\n        },\n        {\n          \"description\": \"The ID of the project you want to add a tag to.\"\n        }\n      ]\n    },\n    \"tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Tags\"\n        },\n        {\n          \"description\": \"The tags you want to add to the project.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"id\",\n    \"tags\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codestar/refs/heads/main/json-schema/codestar-tag-project-request-schema.json
tags:
- AWS
- Developer Tools
- DevOps
- Project Management
- Team Collaboration
title: TagProjectRequest
---
