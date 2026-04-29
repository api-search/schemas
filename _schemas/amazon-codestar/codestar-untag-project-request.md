---
description: UntagProjectRequest schema from AWS CodeStar API
layout: schema
name: UntagProjectRequest
properties_list:
- description: ''
  name: id
  type: object
- description: ''
  name: tags
  type: object
provider_name: Amazon CodeStar
provider_slug: amazon-codestar
schema_file: json-schema/codestar-untag-project-request-schema.json
slug: codestar-untag-project-request
source_filename: codestar-untag-project-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codestar/refs/heads/main/json-schema/codestar-untag-project-request-schema.json\",\n  \"title\": \"UntagProjectRequest\",\n  \"description\": \"UntagProjectRequest schema from AWS CodeStar API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ProjectId\"\n        },\n        {\n          \"description\": \"The ID of the project to remove tags from.\"\n        }\n      ]\n    },\n    \"tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TagKeys\"\n        },\n        {\n          \"description\": \"The tags to remove from the project.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"id\",\n    \"tags\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codestar/refs/heads/main/json-schema/codestar-untag-project-request-schema.json
tags:
- AWS
- Developer Tools
- DevOps
- Project Management
- Team Collaboration
title: UntagProjectRequest
---
