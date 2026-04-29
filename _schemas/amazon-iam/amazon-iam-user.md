---
description: Schema representing an AWS Identity and Access Management (IAM) user resource.
layout: schema
name: AWS IAM User
properties_list:
- description: The path to the user. For more information about paths, see IAM identifiers in the IAM User Guide.
  name: Path
  type: string
- description: The friendly name identifying the user.
  name: UserName
  type: string
- description: The stable and unique string identifying the user. For more information about IDs, see IAM identifiers in the IAM User Guide.
  name: UserId
  type: string
- description: The Amazon Resource Name (ARN) that identifies the user.
  name: Arn
  type: string
- description: The date and time, in ISO 8601 date-time format, when the user was created.
  name: CreateDate
  type: string
- description: The date and time, in ISO 8601 date-time format, when the user's password was last used to sign in to an AWS website.
  name: PasswordLastUsed
  type:
  - string
  - 'null'
- description: The ARN of the policy used to set the permissions boundary for the user.
  name: PermissionsBoundary
  type: object
- description: A list of tags attached to the user.
  name: Tags
  type: array
provider_name: Amazon IAM
provider_slug: amazon-iam
schema_file: json-schema/amazon-iam-user-schema.json
slug: amazon-iam-user
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api.apis.guru/schemas/amazonaws.com/iam/user.json\",\n  \"title\": \"AWS IAM User\",\n  \"description\": \"Schema representing an AWS Identity and Access Management (IAM) user resource.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Path\": {\n      \"type\": \"string\",\n      \"description\": \"The path to the user. For more information about paths, see IAM identifiers in the IAM User Guide.\",\n      \"pattern\": \"^(/[A-Za-z0-9/_-]*)?/$\",\n      \"default\": \"/\"\n    },\n    \"UserName\": {\n      \"type\": \"string\",\n      \"description\": \"The friendly name identifying the user.\",\n      \"minLength\": 1,\n      \"maxLength\": 64,\n      \"pattern\": \"^[\\\\w+=,.@-]+$\"\n    },\n    \"UserId\": {\n      \"type\": \"string\",\n      \"description\": \"The stable and unique string identifying the user. For more information about IDs, see IAM identifiers in the IAM\
  \ User Guide.\",\n      \"pattern\": \"^AIDA[A-Z0-9]+$\"\n    },\n    \"Arn\": {\n      \"type\": \"string\",\n      \"description\": \"The Amazon Resource Name (ARN) that identifies the user.\",\n      \"pattern\": \"^arn:aws:iam::\\\\d{12}:user(/[\\\\w+=,.@/-]+)+$\"\n    },\n    \"CreateDate\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The date and time, in ISO 8601 date-time format, when the user was created.\"\n    },\n    \"PasswordLastUsed\": {\n      \"type\": [\"string\", \"null\"],\n      \"format\": \"date-time\",\n      \"description\": \"The date and time, in ISO 8601 date-time format, when the user's password was last used to sign in to an AWS website.\"\n    },\n    \"PermissionsBoundary\": {\n      \"type\": \"object\",\n      \"description\": \"The ARN of the policy used to set the permissions boundary for the user.\",\n      \"properties\": {\n        \"PermissionsBoundaryType\": {\n          \"type\": \"string\",\n    \
  \      \"enum\": [\"PermissionsBoundaryPolicy\"],\n          \"description\": \"The permissions boundary usage type.\"\n        },\n        \"PermissionsBoundaryArn\": {\n          \"type\": \"string\",\n          \"description\": \"The ARN of the policy used to set the permissions boundary.\"\n        }\n      },\n      \"required\": [\"PermissionsBoundaryType\", \"PermissionsBoundaryArn\"]\n    },\n    \"Tags\": {\n      \"type\": \"array\",\n      \"description\": \"A list of tags attached to the user.\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"Key\": {\n            \"type\": \"string\",\n            \"description\": \"The key name for the tag.\",\n            \"minLength\": 1,\n            \"maxLength\": 128\n          },\n          \"Value\": {\n            \"type\": \"string\",\n            \"description\": \"The value associated with the tag.\",\n            \"maxLength\": 256\n          }\n        },\n        \"required\": [\"\
  Key\", \"Value\"]\n      },\n      \"maxItems\": 50\n    }\n  },\n  \"required\": [\"UserName\", \"UserId\", \"Arn\", \"CreateDate\"],\n  \"additionalProperties\": false\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iam/refs/heads/main/json-schema/amazon-iam-user-schema.json
tags:
- Access Management
- Authentication
- Authorization
- AWS
- Identity
- Security
title: AWS IAM User
---
