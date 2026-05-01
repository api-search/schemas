---
description: Represents the request to verify user attributes.
layout: schema
name: VerifyUserAttributeRequest
properties_list:
- description: ''
  name: AccessToken
  type: object
- description: ''
  name: AttributeName
  type: object
- description: ''
  name: Code
  type: object
provider_name: Amazon Cognito
provider_slug: aws-cognito
schema_file: json-schema/cognito-idp-verify-user-attribute-request-schema.json
slug: cognito-idp-verify-user-attribute-request
source_filename: cognito-idp-verify-user-attribute-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"AccessToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TokenModelType\"\n        },\n        {\n          \"description\": \"A valid access token that Amazon Cognito issued to the user whose user attributes you want to verify.\"\n        }\n      ]\n    },\n    \"AttributeName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AttributeNameType\"\n        },\n        {\n          \"description\": \"The attribute name in the request to verify user attributes.\"\n        }\n      ]\n    },\n    \"Code\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ConfirmationCodeType\"\n        },\n        {\n          \"description\": \"The verification code in the request to verify user attributes.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"AccessToken\",\n    \"AttributeName\",\n    \"Code\"\n  ],\n  \"description\": \"\
  Represents the request to verify user attributes.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-cognito/refs/heads/main/json-schema/cognito-idp-verify-user-attribute-request-schema.json\",\n  \"title\": \"VerifyUserAttributeRequest\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-cognito/refs/heads/main/json-schema/cognito-idp-verify-user-attribute-request-schema.json
tags:
- Authentication
- Authorization
- Identity
- Identity Provider
- OAuth2
- OIDC
title: VerifyUserAttributeRequest
---
