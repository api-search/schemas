---
description: AssociateTeamMemberRequest schema from AWS CodeStar API
layout: schema
name: AssociateTeamMemberRequest
properties_list:
- description: ''
  name: projectId
  type: object
- description: ''
  name: clientRequestToken
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
schema_file: json-schema/codestar-associate-team-member-request-schema.json
slug: codestar-associate-team-member-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codestar/refs/heads/main/json-schema/codestar-associate-team-member-request-schema.json\",\n  \"title\": \"AssociateTeamMemberRequest\",\n  \"description\": \"AssociateTeamMemberRequest schema from AWS CodeStar API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"projectId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ProjectId\"\n        },\n        {\n          \"description\": \"The ID of the project to which you will add the IAM user.\"\n        }\n      ]\n    },\n    \"clientRequestToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ClientRequestToken\"\n        },\n        {\n          \"description\": \"A user- or system-generated token that identifies the entity that requested the team member association to the project. This token can be used to repeat the\
  \ request.\"\n        }\n      ]\n    },\n    \"userArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UserArn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) for the IAM user you want to add to the AWS CodeStar project.\"\n        }\n      ]\n    },\n    \"projectRole\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Role\"\n        },\n        {\n          \"description\": \"The AWS CodeStar project role that will apply to this user. This role determines what actions a user can take in an AWS CodeStar project.\"\n        }\n      ]\n    },\n    \"remoteAccessAllowed\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RemoteAccessAllowed\"\n        },\n        {\n          \"description\": \"Whether the team member is allowed to use an SSH public/private key pair to remotely access project resources, for example Amazon EC2 instances.\"\n        }\n      ]\n\
  \    }\n  },\n  \"required\": [\n    \"projectId\",\n    \"userArn\",\n    \"projectRole\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codestar/refs/heads/main/json-schema/codestar-associate-team-member-request-schema.json
tags:
- AWS
- Developer Tools
- DevOps
- Project Management
- Team Collaboration
title: AssociateTeamMemberRequest
---
