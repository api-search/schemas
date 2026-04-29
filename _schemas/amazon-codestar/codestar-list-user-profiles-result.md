---
description: ListUserProfilesResult schema from AWS CodeStar API
layout: schema
name: ListUserProfilesResult
properties_list:
- description: ''
  name: userProfiles
  type: object
- description: ''
  name: nextToken
  type: object
provider_name: Amazon CodeStar
provider_slug: amazon-codestar
schema_file: json-schema/codestar-list-user-profiles-result-schema.json
slug: codestar-list-user-profiles-result
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codestar/refs/heads/main/json-schema/codestar-list-user-profiles-result-schema.json\",\n  \"title\": \"ListUserProfilesResult\",\n  \"description\": \"ListUserProfilesResult schema from AWS CodeStar API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"userProfiles\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UserProfilesList\"\n        },\n        {\n          \"description\": \"All the user profiles configured in AWS CodeStar for an AWS account.\"\n        }\n      ]\n    },\n    \"nextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PaginationToken\"\n        },\n        {\n          \"description\": \"The continuation token to use when requesting the next set of results, if there are more results to be returned.\"\n        }\n      ]\n    }\n  },\n  \"required\"\
  : [\n    \"userProfiles\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codestar/refs/heads/main/json-schema/codestar-list-user-profiles-result-schema.json
tags:
- AWS
- Developer Tools
- DevOps
- Project Management
- Team Collaboration
title: ListUserProfilesResult
---
