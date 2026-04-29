---
description: CreateRoleResponse schema from AWS IAM API
layout: schema
name: CreateRoleResponse
properties_list:
- description: ''
  name: CreateRoleResult
  type: object
provider_name: Amazon IAM
provider_slug: amazon-iam
schema_file: json-schema/amazon-iam-create-role-response-schema.json
slug: amazon-iam-create-role-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iam/refs/heads/main/json-schema/amazon-iam-create-role-response-schema.json\",\n  \"title\": \"CreateRoleResponse\",\n  \"description\": \"CreateRoleResponse schema from AWS IAM API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"CreateRoleResult\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"Role\": {\n          \"$ref\": \"#/components/schemas/Role\"\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iam/refs/heads/main/json-schema/amazon-iam-create-role-response-schema.json
tags:
- Access Management
- Authentication
- Authorization
- AWS
- Identity
- Security
title: CreateRoleResponse
---
