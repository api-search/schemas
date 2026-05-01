---
description: UpdateTeamMemberResult schema from AWS CodeStar API
layout: schema
name: UpdateTeamMemberResult
properties_list:
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
schema_file: json-schema/codestar-update-team-member-result-schema.json
slug: codestar-update-team-member-result
source_filename: codestar-update-team-member-result-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codestar/refs/heads/main/json-schema/codestar-update-team-member-result-schema.json\",\n  \"title\": \"UpdateTeamMemberResult\",\n  \"description\": \"UpdateTeamMemberResult schema from AWS CodeStar API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"userArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UserArn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the user whose team membership attributes were updated.\"\n        }\n      ]\n    },\n    \"projectRole\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Role\"\n        },\n        {\n          \"description\": \"The project role granted to the user.\"\n        }\n      ]\n    },\n    \"remoteAccessAllowed\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RemoteAccessAllowed\"\
  \n        },\n        {\n          \"description\": \"Whether a team member is allowed to remotely access project resources using the SSH public key associated with the user's profile.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codestar/refs/heads/main/json-schema/codestar-update-team-member-result-schema.json
tags:
- Developer Tools
- DevOps
- Project Management
- Team Collaboration
title: UpdateTeamMemberResult
---
