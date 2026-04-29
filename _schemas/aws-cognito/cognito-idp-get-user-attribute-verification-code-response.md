---
description: The verification code response returned by the server response to get the user attribute verification code.
layout: schema
name: GetUserAttributeVerificationCodeResponse
properties_list:
- description: ''
  name: CodeDeliveryDetails
  type: object
provider_name: Amazon Cognito
provider_slug: aws-cognito
schema_file: json-schema/cognito-idp-get-user-attribute-verification-code-response-schema.json
slug: cognito-idp-get-user-attribute-verification-code-response
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"CodeDeliveryDetails\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CodeDeliveryDetailsType\"\n        },\n        {\n          \"description\": \"The code delivery details returned by the server in response to the request to get the user attribute verification code.\"\n        }\n      ]\n    }\n  },\n  \"description\": \"The verification code response returned by the server response to get the user attribute verification code.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-cognito/refs/heads/main/json-schema/cognito-idp-get-user-attribute-verification-code-response-schema.json\",\n  \"title\": \"GetUserAttributeVerificationCodeResponse\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-cognito/refs/heads/main/json-schema/cognito-idp-get-user-attribute-verification-code-response-schema.json
tags:
- Authentication
- Authorization
- AWS
- Identity
- Identity Provider
- OAuth2
- OIDC
title: GetUserAttributeVerificationCodeResponse
---
