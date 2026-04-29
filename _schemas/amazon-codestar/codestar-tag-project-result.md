---
description: TagProjectResult schema from AWS CodeStar API
layout: schema
name: TagProjectResult
properties_list:
- description: ''
  name: tags
  type: object
provider_name: Amazon CodeStar
provider_slug: amazon-codestar
schema_file: json-schema/codestar-tag-project-result-schema.json
slug: codestar-tag-project-result
source_filename: codestar-tag-project-result-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codestar/refs/heads/main/json-schema/codestar-tag-project-result-schema.json\",\n  \"title\": \"TagProjectResult\",\n  \"description\": \"TagProjectResult schema from AWS CodeStar API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Tags\"\n        },\n        {\n          \"description\": \"The tags for the project.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codestar/refs/heads/main/json-schema/codestar-tag-project-result-schema.json
tags:
- AWS
- Developer Tools
- DevOps
- Project Management
- Team Collaboration
title: TagProjectResult
---
