---
description: ListTagsForProjectResult schema from AWS CodeStar API
layout: schema
name: ListTagsForProjectResult
properties_list:
- description: ''
  name: tags
  type: object
- description: ''
  name: nextToken
  type: object
provider_name: Amazon CodeStar
provider_slug: amazon-codestar
schema_file: json-schema/codestar-list-tags-for-project-result-schema.json
slug: codestar-list-tags-for-project-result
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codestar/refs/heads/main/json-schema/codestar-list-tags-for-project-result-schema.json\",\n  \"title\": \"ListTagsForProjectResult\",\n  \"description\": \"ListTagsForProjectResult schema from AWS CodeStar API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Tags\"\n        },\n        {\n          \"description\": \"The tags for the project.\"\n        }\n      ]\n    },\n    \"nextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PaginationToken\"\n        },\n        {\n          \"description\": \"Reserved for future use.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codestar/refs/heads/main/json-schema/codestar-list-tags-for-project-result-schema.json
tags:
- AWS
- Developer Tools
- DevOps
- Project Management
- Team Collaboration
title: ListTagsForProjectResult
---
