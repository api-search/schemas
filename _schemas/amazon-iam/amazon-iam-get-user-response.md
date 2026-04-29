---
description: GetUserResponse schema from AWS IAM API
layout: schema
name: GetUserResponse
properties_list:
- description: ''
  name: GetUserResult
  type: object
provider_name: Amazon IAM
provider_slug: amazon-iam
schema_file: json-schema/amazon-iam-get-user-response-schema.json
slug: amazon-iam-get-user-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iam/refs/heads/main/json-schema/amazon-iam-get-user-response-schema.json\",\n  \"title\": \"GetUserResponse\",\n  \"description\": \"GetUserResponse schema from AWS IAM API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"GetUserResult\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"User\": {\n          \"$ref\": \"#/components/schemas/User\"\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iam/refs/heads/main/json-schema/amazon-iam-get-user-response-schema.json
tags:
- Access Management
- Authentication
- Authorization
- AWS
- Identity
- Security
title: GetUserResponse
---
