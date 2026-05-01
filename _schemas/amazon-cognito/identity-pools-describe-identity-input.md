---
description: Input to the <code>DescribeIdentity</code> action.
layout: schema
name: DescribeIdentityInput
properties_list:
- description: ''
  name: IdentityId
  type: object
provider_name: Amazon Cognito
provider_slug: amazon-cognito
schema_file: json-schema/identity-pools-describe-identity-input-schema.json
slug: identity-pools-describe-identity-input
source_filename: identity-pools-describe-identity-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-cognito/refs/heads/main/json-schema/identity-pools-describe-identity-input-schema.json\",\n  \"title\": \"DescribeIdentityInput\",\n  \"description\": \"Input to the <code>DescribeIdentity</code> action.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"IdentityId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IdentityId\"\n        },\n        {\n          \"description\": \"A unique identifier in the format REGION:GUID.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"IdentityId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-cognito/refs/heads/main/json-schema/identity-pools-describe-identity-input-schema.json
tags:
- Authentication
- Identity
- OAuth
- User Management
title: DescribeIdentityInput
---
