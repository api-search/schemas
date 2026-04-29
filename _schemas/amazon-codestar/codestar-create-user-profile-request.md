---
description: CreateUserProfileRequest schema from AWS CodeStar API
layout: schema
name: CreateUserProfileRequest
properties_list:
- description: ''
  name: userArn
  type: object
- description: ''
  name: displayName
  type: object
- description: ''
  name: emailAddress
  type: object
- description: ''
  name: sshPublicKey
  type: object
provider_name: Amazon CodeStar
provider_slug: amazon-codestar
schema_file: json-schema/codestar-create-user-profile-request-schema.json
slug: codestar-create-user-profile-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codestar/refs/heads/main/json-schema/codestar-create-user-profile-request-schema.json\",\n  \"title\": \"CreateUserProfileRequest\",\n  \"description\": \"CreateUserProfileRequest schema from AWS CodeStar API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"userArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UserArn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the user in IAM.\"\n        }\n      ]\n    },\n    \"displayName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UserProfileDisplayName\"\n        },\n        {\n          \"description\": \"The name that will be displayed as the friendly name for the user in AWS CodeStar. \"\n        }\n      ]\n    },\n    \"emailAddress\": {\n      \"allOf\": [\n        {\n    \
  \      \"$ref\": \"#/components/schemas/Email\"\n        },\n        {\n          \"description\": \"The email address that will be displayed as part of the user's profile in AWS CodeStar.\"\n        }\n      ]\n    },\n    \"sshPublicKey\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SshPublicKey\"\n        },\n        {\n          \"description\": \"The SSH public key associated with the user in AWS CodeStar. If a project owner allows the user remote access to project resources, this public key will be used along with the user's private key for SSH access.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"userArn\",\n    \"displayName\",\n    \"emailAddress\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codestar/refs/heads/main/json-schema/codestar-create-user-profile-request-schema.json
tags:
- AWS
- Developer Tools
- DevOps
- Project Management
- Team Collaboration
title: CreateUserProfileRequest
---
