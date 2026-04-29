---
description: GetRoleResponse schema from AWS IAM API
layout: schema
name: GetRoleResponse
properties_list:
- description: ''
  name: GetRoleResult
  type: object
provider_name: Amazon IAM
provider_slug: amazon-iam
schema_file: json-schema/amazon-iam-get-role-response-schema.json
slug: amazon-iam-get-role-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iam/refs/heads/main/json-schema/amazon-iam-get-role-response-schema.json\",\n  \"title\": \"GetRoleResponse\",\n  \"description\": \"GetRoleResponse schema from AWS IAM API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"GetRoleResult\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"Role\": {\n          \"$ref\": \"#/components/schemas/Role\"\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iam/refs/heads/main/json-schema/amazon-iam-get-role-response-schema.json
tags:
- Access Management
- Authentication
- Authorization
- AWS
- Identity
- Security
title: GetRoleResponse
---
