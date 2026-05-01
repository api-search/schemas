---
description: UpdateUserProfileResult schema from AWS CodeStar API
layout: schema
name: UpdateUserProfileResult
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
- description: ''
  name: createdTimestamp
  type: object
- description: ''
  name: lastModifiedTimestamp
  type: object
provider_name: Amazon CodeStar
provider_slug: amazon-codestar
schema_file: json-schema/codestar-update-user-profile-result-schema.json
slug: codestar-update-user-profile-result
source_filename: codestar-update-user-profile-result-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codestar/refs/heads/main/json-schema/codestar-update-user-profile-result-schema.json\",\n  \"title\": \"UpdateUserProfileResult\",\n  \"description\": \"UpdateUserProfileResult schema from AWS CodeStar API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"userArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UserArn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the user in IAM.\"\n        }\n      ]\n    },\n    \"displayName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UserProfileDisplayName\"\n        },\n        {\n          \"description\": \"The name that is displayed as the friendly name for the user in AWS CodeStar.\"\n        }\n      ]\n    },\n    \"emailAddress\": {\n      \"allOf\": [\n        {\n          \"$ref\"\
  : \"#/components/schemas/Email\"\n        },\n        {\n          \"description\": \"The email address that is displayed as part of the user's profile in AWS CodeStar.\"\n        }\n      ]\n    },\n    \"sshPublicKey\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SshPublicKey\"\n        },\n        {\n          \"description\": \"The SSH public key associated with the user in AWS CodeStar. This is the public portion of the public/private keypair the user can use to access project resources if a project owner allows the user remote access to those resources.\"\n        }\n      ]\n    },\n    \"createdTimestamp\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CreatedTimestamp\"\n        },\n        {\n          \"description\": \"The date the user profile was created, in timestamp format.\"\n        }\n      ]\n    },\n    \"lastModifiedTimestamp\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LastModifiedTimestamp\"\
  \n        },\n        {\n          \"description\": \"The date the user profile was last modified, in timestamp format.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"userArn\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codestar/refs/heads/main/json-schema/codestar-update-user-profile-result-schema.json
tags:
- Developer Tools
- DevOps
- Project Management
- Team Collaboration
title: UpdateUserProfileResult
---
