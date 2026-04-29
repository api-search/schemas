---
description: CreateAccessKeyResponse schema from AWS IAM API
layout: schema
name: CreateAccessKeyResponse
properties_list:
- description: ''
  name: CreateAccessKeyResult
  type: object
provider_name: Amazon IAM
provider_slug: amazon-iam
schema_file: json-schema/amazon-iam-create-access-key-response-schema.json
slug: amazon-iam-create-access-key-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iam/refs/heads/main/json-schema/amazon-iam-create-access-key-response-schema.json\",\n  \"title\": \"CreateAccessKeyResponse\",\n  \"description\": \"CreateAccessKeyResponse schema from AWS IAM API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"CreateAccessKeyResult\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"AccessKey\": {\n          \"$ref\": \"#/components/schemas/AccessKey\"\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iam/refs/heads/main/json-schema/amazon-iam-create-access-key-response-schema.json
tags:
- Access Management
- Authentication
- Authorization
- AWS
- Identity
- Security
title: CreateAccessKeyResponse
---
