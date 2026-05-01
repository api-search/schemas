---
description: ListTeamMembersRequest schema from AWS CodeStar API
layout: schema
name: ListTeamMembersRequest
properties_list:
- description: ''
  name: projectId
  type: object
- description: ''
  name: nextToken
  type: object
- description: ''
  name: maxResults
  type: object
provider_name: Amazon CodeStar
provider_slug: amazon-codestar
schema_file: json-schema/codestar-list-team-members-request-schema.json
slug: codestar-list-team-members-request
source_filename: codestar-list-team-members-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codestar/refs/heads/main/json-schema/codestar-list-team-members-request-schema.json\",\n  \"title\": \"ListTeamMembersRequest\",\n  \"description\": \"ListTeamMembersRequest schema from AWS CodeStar API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"projectId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ProjectId\"\n        },\n        {\n          \"description\": \"The ID of the project for which you want to list team members.\"\n        }\n      ]\n    },\n    \"nextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PaginationToken\"\n        },\n        {\n          \"description\": \"The continuation token for the next set of results, if the results cannot be returned in one response.\"\n        }\n      ]\n    },\n    \"maxResults\": {\n      \"allOf\": [\n\
  \        {\n          \"$ref\": \"#/components/schemas/MaxResults\"\n        },\n        {\n          \"description\": \"The maximum number of team members you want returned in a response.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"projectId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codestar/refs/heads/main/json-schema/codestar-list-team-members-request-schema.json
tags:
- Developer Tools
- DevOps
- Project Management
- Team Collaboration
title: ListTeamMembersRequest
---
