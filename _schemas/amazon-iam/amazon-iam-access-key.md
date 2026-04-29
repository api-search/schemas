---
description: AccessKey schema from AWS IAM API
layout: schema
name: AccessKey
properties_list:
- description: The name of the IAM user the access key is associated with.
  name: UserName
  type: string
- description: The ID for this access key.
  name: AccessKeyId
  type: string
- description: The status of the access key.
  name: Status
  type: string
- description: The secret key used to sign requests. Only returned on creation.
  name: SecretAccessKey
  type: string
- description: The date when the access key was created.
  name: CreateDate
  type: string
provider_name: Amazon IAM
provider_slug: amazon-iam
schema_file: json-schema/amazon-iam-access-key-schema.json
slug: amazon-iam-access-key
source_filename: amazon-iam-access-key-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iam/refs/heads/main/json-schema/amazon-iam-access-key-schema.json\",\n  \"title\": \"AccessKey\",\n  \"description\": \"AccessKey schema from AWS IAM API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"UserName\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the IAM user the access key is associated with.\"\n    },\n    \"AccessKeyId\": {\n      \"type\": \"string\",\n      \"description\": \"The ID for this access key.\"\n    },\n    \"Status\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"Active\",\n        \"Inactive\"\n      ],\n      \"description\": \"The status of the access key.\"\n    },\n    \"SecretAccessKey\": {\n      \"type\": \"string\",\n      \"description\": \"The secret key used to sign requests. Only returned on creation.\"\n    },\n    \"CreateDate\": {\n      \"type\":\
  \ \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The date when the access key was created.\"\n    }\n  },\n  \"required\": [\n    \"UserName\",\n    \"AccessKeyId\",\n    \"Status\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iam/refs/heads/main/json-schema/amazon-iam-access-key-schema.json
tags:
- Access Management
- Authentication
- Authorization
- AWS
- Identity
- Security
title: AccessKey
---
