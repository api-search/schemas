---
description: Represents the response to describe the user pool.
layout: schema
name: DescribeUserPoolResponse
properties_list:
- description: ''
  name: UserPool
  type: object
provider_name: Amazon Cognito
provider_slug: amazon-cognito
schema_file: json-schema/user-pools-describe-user-pool-response-schema.json
slug: user-pools-describe-user-pool-response
source_filename: user-pools-describe-user-pool-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-cognito/refs/heads/main/json-schema/user-pools-describe-user-pool-response-schema.json\",\n  \"title\": \"DescribeUserPoolResponse\",\n  \"description\": \"Represents the response to describe the user pool.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"UserPool\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UserPoolType\"\n        },\n        {\n          \"description\": \"The container of metadata returned by the server to describe the pool.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-cognito/refs/heads/main/json-schema/user-pools-describe-user-pool-response-schema.json
tags:
- Authentication
- Identity
- OAuth
- User Management
title: DescribeUserPoolResponse
---
