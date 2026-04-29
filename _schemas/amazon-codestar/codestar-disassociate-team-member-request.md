---
description: DisassociateTeamMemberRequest schema from AWS CodeStar API
layout: schema
name: DisassociateTeamMemberRequest
properties_list:
- description: ''
  name: projectId
  type: object
- description: ''
  name: userArn
  type: object
provider_name: Amazon CodeStar
provider_slug: amazon-codestar
schema_file: json-schema/codestar-disassociate-team-member-request-schema.json
slug: codestar-disassociate-team-member-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codestar/refs/heads/main/json-schema/codestar-disassociate-team-member-request-schema.json\",\n  \"title\": \"DisassociateTeamMemberRequest\",\n  \"description\": \"DisassociateTeamMemberRequest schema from AWS CodeStar API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"projectId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ProjectId\"\n        },\n        {\n          \"description\": \"The ID of the AWS CodeStar project from which you want to remove a team member.\"\n        }\n      ]\n    },\n    \"userArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UserArn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the IAM user or group whom you want to remove from the project.\"\n        }\n      ]\n    }\n  },\n  \"required\"\
  : [\n    \"projectId\",\n    \"userArn\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codestar/refs/heads/main/json-schema/codestar-disassociate-team-member-request-schema.json
tags:
- AWS
- Developer Tools
- DevOps
- Project Management
- Team Collaboration
title: DisassociateTeamMemberRequest
---
