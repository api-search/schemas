---
description: Input to the <code>GetOpenIdTokenForDeveloperIdentity</code> action.
layout: schema
name: GetOpenIdTokenForDeveloperIdentityInput
properties_list:
- description: ''
  name: IdentityPoolId
  type: object
- description: ''
  name: IdentityId
  type: object
- description: ''
  name: Logins
  type: object
- description: ''
  name: PrincipalTags
  type: object
- description: ''
  name: TokenDuration
  type: object
provider_name: Amazon Cognito
provider_slug: aws-cognito
schema_file: json-schema/cognito-identity-get-open-id-token-for-developer-identity-input-schema.json
slug: cognito-identity-get-open-id-token-for-developer-identity-input
source_filename: cognito-identity-get-open-id-token-for-developer-identity-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"IdentityPoolId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IdentityPoolId\"\n        },\n        {\n          \"description\": \"An identity pool ID in the format REGION:GUID.\"\n        }\n      ]\n    },\n    \"IdentityId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IdentityId\"\n        },\n        {\n          \"description\": \"A unique identifier in the format REGION:GUID.\"\n        }\n      ]\n    },\n    \"Logins\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LoginsMap\"\n        },\n        {\n          \"description\": \"A set of optional name-value pairs that map provider names to provider tokens. Each name-value pair represents a user from a public provider or developer provider. If the user is from a developer provider, the name-value pair will follow the syntax <code>\\\"developer_provider_name\\\": \\\"\
  developer_user_identifier\\\"</code>. The developer provider is the \\\"domain\\\" by which Cognito will refer to your users; you provided this domain while creating/updating the identity pool. The developer user identifier is an identifier from your backend that uniquely identifies a user. When you create an identity pool, you can specify the supported logins.\"\n        }\n      ]\n    },\n    \"PrincipalTags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PrincipalTags\"\n        },\n        {\n          \"description\": \"Use this operation to configure attribute mappings for custom providers. \"\n        }\n      ]\n    },\n    \"TokenDuration\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TokenDuration\"\n        },\n        {\n          \"description\": \"<p>The expiration time of the token, in seconds. You can specify a custom expiration time for the token so that you can cache it. If you don't provide an expiration\
  \ time, the token is valid for 15 minutes. You can exchange the token with Amazon STS for temporary AWS credentials, which are valid for a maximum of one hour. The maximum token duration you can set is 24 hours. You should take care in setting the expiration time for a token, as there are significant security implications: an attacker could use a leaked token to access your AWS resources for the token's duration.</p> <note> <p>Please provide for a small grace period, usually no more than 5 minutes, to account for clock skew.</p> </note>\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"IdentityPoolId\",\n    \"Logins\"\n  ],\n  \"description\": \"Input to the <code>GetOpenIdTokenForDeveloperIdentity</code> action.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-cognito/refs/heads/main/json-schema/cognito-identity-get-open-id-token-for-developer-identity-input-schema.json\",\n  \"title\":\
  \ \"GetOpenIdTokenForDeveloperIdentityInput\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-cognito/refs/heads/main/json-schema/cognito-identity-get-open-id-token-for-developer-identity-input-schema.json
tags:
- Authentication
- Authorization
- Identity
- Identity Provider
- OAuth2
- OIDC
title: GetOpenIdTokenForDeveloperIdentityInput
---
