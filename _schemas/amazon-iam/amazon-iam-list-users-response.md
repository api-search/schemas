---
description: ListUsersResponse schema from AWS IAM API
layout: schema
name: ListUsersResponse
properties_list:
- description: ''
  name: ListUsersResult
  type: object
provider_name: Amazon IAM
provider_slug: amazon-iam
schema_file: json-schema/amazon-iam-list-users-response-schema.json
slug: amazon-iam-list-users-response
source_filename: amazon-iam-list-users-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iam/refs/heads/main/json-schema/amazon-iam-list-users-response-schema.json\",\n  \"title\": \"ListUsersResponse\",\n  \"description\": \"ListUsersResponse schema from AWS IAM API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ListUsersResult\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"Users\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"$ref\": \"#/components/schemas/User\"\n          }\n        },\n        \"IsTruncated\": {\n          \"type\": \"boolean\"\n        },\n        \"Marker\": {\n          \"type\": \"string\"\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iam/refs/heads/main/json-schema/amazon-iam-list-users-response-schema.json
tags:
- Access Management
- Authentication
- Authorization
- Identity
- Security
title: ListUsersResponse
---
