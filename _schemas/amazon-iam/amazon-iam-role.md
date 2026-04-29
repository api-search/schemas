---
description: Role schema from AWS IAM API
layout: schema
name: Role
properties_list:
- description: The path to the role.
  name: Path
  type: string
- description: The friendly name that identifies the role.
  name: RoleName
  type: string
- description: The stable and unique string identifying the role.
  name: RoleId
  type: string
- description: The Amazon Resource Name (ARN) specifying the role.
  name: Arn
  type: string
- description: The date and time when the role was created.
  name: CreateDate
  type: string
- description: The policy that grants an entity permission to assume the role.
  name: AssumeRolePolicyDocument
  type: string
- description: A description of the role.
  name: Description
  type: string
- description: The maximum session duration (in seconds) for the specified role.
  name: MaxSessionDuration
  type: integer
- description: ''
  name: Tags
  type: array
provider_name: Amazon IAM
provider_slug: amazon-iam
schema_file: json-schema/amazon-iam-role-schema.json
slug: amazon-iam-role
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iam/refs/heads/main/json-schema/amazon-iam-role-schema.json\",\n  \"title\": \"Role\",\n  \"description\": \"Role schema from AWS IAM API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Path\": {\n      \"type\": \"string\",\n      \"description\": \"The path to the role.\"\n    },\n    \"RoleName\": {\n      \"type\": \"string\",\n      \"description\": \"The friendly name that identifies the role.\"\n    },\n    \"RoleId\": {\n      \"type\": \"string\",\n      \"description\": \"The stable and unique string identifying the role.\"\n    },\n    \"Arn\": {\n      \"type\": \"string\",\n      \"description\": \"The Amazon Resource Name (ARN) specifying the role.\"\n    },\n    \"CreateDate\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The date and time when the role was created.\"\n\
  \    },\n    \"AssumeRolePolicyDocument\": {\n      \"type\": \"string\",\n      \"description\": \"The policy that grants an entity permission to assume the role.\"\n    },\n    \"Description\": {\n      \"type\": \"string\",\n      \"description\": \"A description of the role.\"\n    },\n    \"MaxSessionDuration\": {\n      \"type\": \"integer\",\n      \"description\": \"The maximum session duration (in seconds) for the specified role.\"\n    },\n    \"Tags\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/Tag\"\n      }\n    }\n  },\n  \"required\": [\n    \"RoleName\",\n    \"RoleId\",\n    \"Arn\",\n    \"CreateDate\",\n    \"AssumeRolePolicyDocument\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iam/refs/heads/main/json-schema/amazon-iam-role-schema.json
tags:
- Access Management
- Authentication
- Authorization
- AWS
- Identity
- Security
title: Role
---
