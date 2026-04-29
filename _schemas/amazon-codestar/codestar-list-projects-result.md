---
description: ListProjectsResult schema from AWS CodeStar API
layout: schema
name: ListProjectsResult
properties_list:
- description: ''
  name: projects
  type: object
- description: ''
  name: nextToken
  type: object
provider_name: Amazon CodeStar
provider_slug: amazon-codestar
schema_file: json-schema/codestar-list-projects-result-schema.json
slug: codestar-list-projects-result
source_filename: codestar-list-projects-result-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codestar/refs/heads/main/json-schema/codestar-list-projects-result-schema.json\",\n  \"title\": \"ListProjectsResult\",\n  \"description\": \"ListProjectsResult schema from AWS CodeStar API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"projects\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ProjectsList\"\n        },\n        {\n          \"description\": \"A list of projects.\"\n        }\n      ]\n    },\n    \"nextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PaginationToken\"\n        },\n        {\n          \"description\": \"The continuation token to use when requesting the next set of results, if there are more results to be returned.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"projects\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codestar/refs/heads/main/json-schema/codestar-list-projects-result-schema.json
tags:
- AWS
- Developer Tools
- DevOps
- Project Management
- Team Collaboration
title: ListProjectsResult
---
