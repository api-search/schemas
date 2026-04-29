---
description: ListTeamMembersResult schema from AWS CodeStar API
layout: schema
name: ListTeamMembersResult
properties_list:
- description: ''
  name: teamMembers
  type: object
- description: ''
  name: nextToken
  type: object
provider_name: Amazon CodeStar
provider_slug: amazon-codestar
schema_file: json-schema/codestar-list-team-members-result-schema.json
slug: codestar-list-team-members-result
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codestar/refs/heads/main/json-schema/codestar-list-team-members-result-schema.json\",\n  \"title\": \"ListTeamMembersResult\",\n  \"description\": \"ListTeamMembersResult schema from AWS CodeStar API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"teamMembers\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TeamMemberResult\"\n        },\n        {\n          \"description\": \"A list of team member objects for the project.\"\n        }\n      ]\n    },\n    \"nextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PaginationToken\"\n        },\n        {\n          \"description\": \"The continuation token to use when requesting the next set of results, if there are more results to be returned.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"teamMembers\"\
  \n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codestar/refs/heads/main/json-schema/codestar-list-team-members-result-schema.json
tags:
- AWS
- Developer Tools
- DevOps
- Project Management
- Team Collaboration
title: ListTeamMembersResult
---
