---
description: Information about a team member in a project.
layout: schema
name: TeamMember
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
schema_file: json-schema/codestar-team-member-schema.json
slug: codestar-team-member
source_filename: codestar-team-member-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codestar/refs/heads/main/json-schema/codestar-team-member-schema.json\",\n  \"title\": \"TeamMember\",\n  \"description\": \"Information about a team member in a project.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"userArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UserArn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the user in IAM.\"\n        }\n      ]\n    },\n    \"projectRole\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Role\"\n        },\n        {\n          \"description\": \"The role assigned to the user in the project. Project roles have different levels of access. For more information, see <a href=\\\"http://docs.aws.amazon.com/codestar/latest/userguide/working-with-teams.html\\\">Working with Teams</a>\
  \ in the <i>AWS CodeStar User Guide</i>. \"\n        }\n      ]\n    },\n    \"remoteAccessAllowed\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RemoteAccessAllowed\"\n        },\n        {\n          \"description\": \"Whether the user is allowed to remotely access project resources using an SSH public/private key pair.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"userArn\",\n    \"projectRole\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codestar/refs/heads/main/json-schema/codestar-team-member-schema.json
tags:
- Developer Tools
- DevOps
- Project Management
- Team Collaboration
title: TeamMember
---
