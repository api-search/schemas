---
description: Information about a user's profile in AWS CodeStar.
layout: schema
name: UserProfileSummary
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
schema_file: json-schema/codestar-user-profile-summary-schema.json
slug: codestar-user-profile-summary
source_filename: codestar-user-profile-summary-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codestar/refs/heads/main/json-schema/codestar-user-profile-summary-schema.json\",\n  \"title\": \"UserProfileSummary\",\n  \"description\": \"Information about a user's profile in AWS CodeStar.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"userArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UserArn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the user in IAM.\"\n        }\n      ]\n    },\n    \"displayName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UserProfileDisplayName\"\n        },\n        {\n          \"description\": \"The display name of a user in AWS CodeStar. For example, this could be set to both first and last name (\\\"Mary Major\\\") or a single name (\\\"Mary\\\"). The display name is also used to generate\
  \ the initial icon associated with the user in AWS CodeStar projects. If spaces are included in the display name, the first character that appears after the space will be used as the second character in the user initial icon. The initial icon displays a maximum of two characters, so a display name with more than one space (for example \\\"Mary Jane Major\\\") would generate an initial icon using the first character and the first character after the space (\\\"MJ\\\", not \\\"MM\\\").\"\n        }\n      ]\n    },\n    \"emailAddress\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Email\"\n        },\n        {\n          \"description\": \"The email address associated with the user.\"\n        }\n      ]\n    },\n    \"sshPublicKey\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SshPublicKey\"\n        },\n        {\n          \"description\": \"The SSH public key associated with the user in AWS CodeStar. If a project owner\
  \ allows the user remote access to project resources, this public key will be used along with the user's private key for SSH access.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codestar/refs/heads/main/json-schema/codestar-user-profile-summary-schema.json
tags:
- Developer Tools
- DevOps
- Project Management
- Team Collaboration
title: UserProfileSummary
---
