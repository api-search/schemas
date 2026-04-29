---
description: Represents the response from the server from a request to describe the user pool client.
layout: schema
name: DescribeUserPoolClientResponse
properties_list:
- description: ''
  name: UserPoolClient
  type: object
provider_name: Amazon Cognito
provider_slug: amazon-cognito
schema_file: json-schema/user-pools-describe-user-pool-client-response-schema.json
slug: user-pools-describe-user-pool-client-response
source_filename: user-pools-describe-user-pool-client-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-cognito/refs/heads/main/json-schema/user-pools-describe-user-pool-client-response-schema.json\",\n  \"title\": \"DescribeUserPoolClientResponse\",\n  \"description\": \"Represents the response from the server from a request to describe the user pool client.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"UserPoolClient\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UserPoolClientType\"\n        },\n        {\n          \"description\": \"The user pool client from a server response to describe the user pool client.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-cognito/refs/heads/main/json-schema/user-pools-describe-user-pool-client-response-schema.json
tags:
- Authentication
- AWS
- Identity
- OAuth
- User Management
title: DescribeUserPoolClientResponse
---
