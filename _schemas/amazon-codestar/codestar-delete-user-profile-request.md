---
description: DeleteUserProfileRequest schema from AWS CodeStar API
layout: schema
name: DeleteUserProfileRequest
properties_list:
- description: ''
  name: userArn
  type: object
provider_name: Amazon CodeStar
provider_slug: amazon-codestar
schema_file: json-schema/codestar-delete-user-profile-request-schema.json
slug: codestar-delete-user-profile-request
source_filename: codestar-delete-user-profile-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codestar/refs/heads/main/json-schema/codestar-delete-user-profile-request-schema.json\",\n  \"title\": \"DeleteUserProfileRequest\",\n  \"description\": \"DeleteUserProfileRequest schema from AWS CodeStar API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"userArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UserArn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the user to delete from AWS CodeStar.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"userArn\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codestar/refs/heads/main/json-schema/codestar-delete-user-profile-request-schema.json
tags:
- Developer Tools
- DevOps
- Project Management
- Team Collaboration
title: DeleteUserProfileRequest
---
