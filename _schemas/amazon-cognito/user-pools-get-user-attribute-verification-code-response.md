---
description: The verification code response returned by the server response to get the user attribute verification code.
layout: schema
name: GetUserAttributeVerificationCodeResponse
properties_list:
- description: ''
  name: CodeDeliveryDetails
  type: object
provider_name: Amazon Cognito
provider_slug: amazon-cognito
schema_file: json-schema/user-pools-get-user-attribute-verification-code-response-schema.json
slug: user-pools-get-user-attribute-verification-code-response
source_filename: user-pools-get-user-attribute-verification-code-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-cognito/refs/heads/main/json-schema/user-pools-get-user-attribute-verification-code-response-schema.json\",\n  \"title\": \"GetUserAttributeVerificationCodeResponse\",\n  \"description\": \"The verification code response returned by the server response to get the user attribute verification code.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"CodeDeliveryDetails\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CodeDeliveryDetailsType\"\n        },\n        {\n          \"description\": \"The code delivery details returned by the server in response to the request to get the user attribute verification code.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-cognito/refs/heads/main/json-schema/user-pools-get-user-attribute-verification-code-response-schema.json
tags:
- Authentication
- Identity
- OAuth
- User Management
title: GetUserAttributeVerificationCodeResponse
---
