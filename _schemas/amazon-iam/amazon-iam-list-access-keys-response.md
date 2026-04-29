---
description: ListAccessKeysResponse schema from AWS IAM API
layout: schema
name: ListAccessKeysResponse
properties_list:
- description: ''
  name: ListAccessKeysResult
  type: object
provider_name: Amazon IAM
provider_slug: amazon-iam
schema_file: json-schema/amazon-iam-list-access-keys-response-schema.json
slug: amazon-iam-list-access-keys-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iam/refs/heads/main/json-schema/amazon-iam-list-access-keys-response-schema.json\",\n  \"title\": \"ListAccessKeysResponse\",\n  \"description\": \"ListAccessKeysResponse schema from AWS IAM API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ListAccessKeysResult\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"AccessKeyMetadata\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"$ref\": \"#/components/schemas/AccessKey\"\n          }\n        },\n        \"IsTruncated\": {\n          \"type\": \"boolean\"\n        },\n        \"Marker\": {\n          \"type\": \"string\"\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iam/refs/heads/main/json-schema/amazon-iam-list-access-keys-response-schema.json
tags:
- Access Management
- Authentication
- Authorization
- AWS
- Identity
- Security
title: ListAccessKeysResponse
---
