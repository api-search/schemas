---
description: Input to the GetId action.
layout: schema
name: GetIdInput
properties_list:
- description: ''
  name: AccountId
  type: object
- description: ''
  name: IdentityPoolId
  type: object
- description: ''
  name: Logins
  type: object
provider_name: Amazon Cognito
provider_slug: aws-cognito
schema_file: json-schema/cognito-identity-get-id-input-schema.json
slug: cognito-identity-get-id-input
source_filename: cognito-identity-get-id-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"AccountId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AccountId\"\n        },\n        {\n          \"description\": \"A standard AWS account ID (9+ digits).\"\n        }\n      ]\n    },\n    \"IdentityPoolId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IdentityPoolId\"\n        },\n        {\n          \"description\": \"An identity pool ID in the format REGION:GUID.\"\n        }\n      ]\n    },\n    \"Logins\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LoginsMap\"\n        },\n        {\n          \"description\": \"<p>A set of optional name-value pairs that map provider names to provider tokens. The available provider names for <code>Logins</code> are as follows:</p> <ul> <li> <p>Facebook: <code>graph.facebook.com</code> </p> </li> <li> <p>Amazon Cognito user pool: <code>cognito-idp.&lt;region&gt;.amazonaws.com/&lt;YOUR_USER_POOL_ID&gt;</code>,\
  \ for example, <code>cognito-idp.us-east-1.amazonaws.com/us-east-1_123456789</code>. </p> </li> <li> <p>Google: <code>accounts.google.com</code> </p> </li> <li> <p>Amazon: <code>www.amazon.com</code> </p> </li> <li> <p>Twitter: <code>api.twitter.com</code> </p> </li> <li> <p>Digits: <code>www.digits.com</code> </p> </li> </ul>\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"IdentityPoolId\"\n  ],\n  \"description\": \"Input to the GetId action.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-cognito/refs/heads/main/json-schema/cognito-identity-get-id-input-schema.json\",\n  \"title\": \"GetIdInput\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-cognito/refs/heads/main/json-schema/cognito-identity-get-id-input-schema.json
tags:
- Authentication
- Authorization
- AWS
- Identity
- Identity Provider
- OAuth2
- OIDC
title: GetIdInput
---
