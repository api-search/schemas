---
description: The response from the server for a registration request.
layout: schema
name: SignUpResponse
properties_list:
- description: ''
  name: UserConfirmed
  type: object
- description: ''
  name: CodeDeliveryDetails
  type: object
- description: ''
  name: UserSub
  type: object
provider_name: Amazon Cognito
provider_slug: aws-cognito
schema_file: json-schema/cognito-idp-sign-up-response-schema.json
slug: cognito-idp-sign-up-response
source_filename: cognito-idp-sign-up-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"UserConfirmed\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BooleanType\"\n        },\n        {\n          \"description\": \"A response from the server indicating that a user registration has been confirmed.\"\n        }\n      ]\n    },\n    \"CodeDeliveryDetails\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CodeDeliveryDetailsType\"\n        },\n        {\n          \"description\": \"The code delivery details returned by the server response to the user registration request.\"\n        }\n      ]\n    },\n    \"UserSub\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StringType\"\n        },\n        {\n          \"description\": \"The UUID of the authenticated user. This isn't the same as <code>username</code>.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"UserConfirmed\",\n    \"UserSub\"\n  ],\n  \"description\"\
  : \"The response from the server for a registration request.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-cognito/refs/heads/main/json-schema/cognito-idp-sign-up-response-schema.json\",\n  \"title\": \"SignUpResponse\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-cognito/refs/heads/main/json-schema/cognito-idp-sign-up-response-schema.json
tags:
- Authentication
- Authorization
- AWS
- Identity
- Identity Provider
- OAuth2
- OIDC
title: SignUpResponse
---
