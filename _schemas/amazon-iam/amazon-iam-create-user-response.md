---
description: CreateUserResponse schema from AWS IAM API
layout: schema
name: CreateUserResponse
properties_list:
- description: ''
  name: CreateUserResult
  type: object
provider_name: Amazon IAM
provider_slug: amazon-iam
schema_file: json-schema/amazon-iam-create-user-response-schema.json
slug: amazon-iam-create-user-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iam/refs/heads/main/json-schema/amazon-iam-create-user-response-schema.json\",\n  \"title\": \"CreateUserResponse\",\n  \"description\": \"CreateUserResponse schema from AWS IAM API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"CreateUserResult\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"User\": {\n          \"$ref\": \"#/components/schemas/User\"\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iam/refs/heads/main/json-schema/amazon-iam-create-user-response-schema.json
tags:
- Access Management
- Authentication
- Authorization
- AWS
- Identity
- Security
title: CreateUserResponse
---
