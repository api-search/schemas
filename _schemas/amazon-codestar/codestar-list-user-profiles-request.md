---
description: ListUserProfilesRequest schema from AWS CodeStar API
layout: schema
name: ListUserProfilesRequest
properties_list:
- description: ''
  name: nextToken
  type: object
- description: ''
  name: maxResults
  type: object
provider_name: Amazon CodeStar
provider_slug: amazon-codestar
schema_file: json-schema/codestar-list-user-profiles-request-schema.json
slug: codestar-list-user-profiles-request
source_filename: codestar-list-user-profiles-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codestar/refs/heads/main/json-schema/codestar-list-user-profiles-request-schema.json\",\n  \"title\": \"ListUserProfilesRequest\",\n  \"description\": \"ListUserProfilesRequest schema from AWS CodeStar API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"nextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PaginationToken\"\n        },\n        {\n          \"description\": \"The continuation token for the next set of results, if the results cannot be returned in one response.\"\n        }\n      ]\n    },\n    \"maxResults\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MaxResults\"\n        },\n        {\n          \"description\": \"The maximum number of results to return in a response.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codestar/refs/heads/main/json-schema/codestar-list-user-profiles-request-schema.json
tags:
- Developer Tools
- DevOps
- Project Management
- Team Collaboration
title: ListUserProfilesRequest
---
