---
description: DescribeUserProfileResult schema from AWS CodeStar API
layout: schema
name: DescribeUserProfileResult
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
schema_file: json-schema/codestar-describe-user-profile-result-schema.json
slug: codestar-describe-user-profile-result
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codestar/refs/heads/main/json-schema/codestar-describe-user-profile-result-schema.json\",\n  \"title\": \"DescribeUserProfileResult\",\n  \"description\": \"DescribeUserProfileResult schema from AWS CodeStar API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"userArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UserArn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the user.\"\n        }\n      ]\n    },\n    \"displayName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UserProfileDisplayName\"\n        },\n        {\n          \"description\": \"The display name shown for the user in AWS CodeStar projects. For example, this could be set to both first and last name (\\\"Mary Major\\\") or a single name (\\\"Mary\\\"). The display\
  \ name is also used to generate the initial icon associated with the user in AWS CodeStar projects. If spaces are included in the display name, the first character that appears after the space will be used as the second character in the user initial icon. The initial icon displays a maximum of two characters, so a display name with more than one space (for example \\\"Mary Jane Major\\\") would generate an initial icon using the first character and the first character after the space (\\\"MJ\\\", not \\\"MM\\\").\"\n        }\n      ]\n    },\n    \"emailAddress\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Email\"\n        },\n        {\n          \"description\": \"The email address for the user. Optional.\"\n        }\n      ]\n    },\n    \"sshPublicKey\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SshPublicKey\"\n        },\n        {\n          \"description\": \"The SSH public key associated with the user. This\
  \ SSH public key is associated with the user profile, and can be used in conjunction with the associated private key for access to project resources, such as Amazon EC2 instances, if a project owner grants remote access to those resources.\"\n        }\n      ]\n    },\n    \"createdTimestamp\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CreatedTimestamp\"\n        },\n        {\n          \"description\": \"The date and time when the user profile was created in AWS CodeStar, in timestamp format.\"\n        }\n      ]\n    },\n    \"lastModifiedTimestamp\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LastModifiedTimestamp\"\n        },\n        {\n          \"description\": \"The date and time when the user profile was last modified, in timestamp format.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"userArn\",\n    \"createdTimestamp\",\n    \"lastModifiedTimestamp\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codestar/refs/heads/main/json-schema/codestar-describe-user-profile-result-schema.json
tags:
- AWS
- Developer Tools
- DevOps
- Project Management
- Team Collaboration
title: DescribeUserProfileResult
---
