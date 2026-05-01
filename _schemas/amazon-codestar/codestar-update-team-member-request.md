---
description: UpdateTeamMemberRequest schema from AWS CodeStar API
layout: schema
name: UpdateTeamMemberRequest
properties_list:
- description: ''
  name: projectId
  type: object
- description: ''
  name: userArn
  type: object
- description: ''
  name: projectRole
  type: object
- description: ''
  name: remoteAccessAllowed
  type: object
provider_name: Amazon CodeStar
provider_slug: amazon-codestar
schema_file: json-schema/codestar-update-team-member-request-schema.json
slug: codestar-update-team-member-request
source_filename: codestar-update-team-member-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codestar/refs/heads/main/json-schema/codestar-update-team-member-request-schema.json\",\n  \"title\": \"UpdateTeamMemberRequest\",\n  \"description\": \"UpdateTeamMemberRequest schema from AWS CodeStar API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"projectId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ProjectId\"\n        },\n        {\n          \"description\": \"The ID of the project.\"\n        }\n      ]\n    },\n    \"userArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UserArn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the user for whom you want to change team membership attributes.\"\n        }\n      ]\n    },\n    \"projectRole\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Role\"\
  \n        },\n        {\n          \"description\": \"The role assigned to the user in the project. Project roles have different levels of access. For more information, see <a href=\\\"http://docs.aws.amazon.com/codestar/latest/userguide/working-with-teams.html\\\">Working with Teams</a> in the <i>AWS CodeStar User Guide</i>.\"\n        }\n      ]\n    },\n    \"remoteAccessAllowed\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RemoteAccessAllowed\"\n        },\n        {\n          \"description\": \"Whether a team member is allowed to remotely access project resources using the SSH public key associated with the user's profile. Even if this is set to True, the user must associate a public key with their profile before the user can access resources.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"projectId\",\n    \"userArn\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codestar/refs/heads/main/json-schema/codestar-update-team-member-request-schema.json
tags:
- Developer Tools
- DevOps
- Project Management
- Team Collaboration
title: UpdateTeamMemberRequest
---
