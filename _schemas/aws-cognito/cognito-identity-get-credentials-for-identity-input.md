---
description: Input to the <code>GetCredentialsForIdentity</code> action.
layout: schema
name: GetCredentialsForIdentityInput
properties_list:
- description: ''
  name: IdentityId
  type: object
- description: ''
  name: Logins
  type: object
- description: ''
  name: CustomRoleArn
  type: object
provider_name: Amazon Cognito
provider_slug: aws-cognito
schema_file: json-schema/cognito-identity-get-credentials-for-identity-input-schema.json
slug: cognito-identity-get-credentials-for-identity-input
source_filename: cognito-identity-get-credentials-for-identity-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"IdentityId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IdentityId\"\n        },\n        {\n          \"description\": \"A unique identifier in the format REGION:GUID.\"\n        }\n      ]\n    },\n    \"Logins\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LoginsMap\"\n        },\n        {\n          \"description\": \"<p>A set of optional name-value pairs that map provider names to provider tokens. The name-value pair will follow the syntax \\\"provider_name\\\": \\\"provider_user_identifier\\\".</p> <p>Logins should not be specified when trying to get credentials for an unauthenticated identity.</p> <p>The Logins parameter is required when using identities associated with external identity providers such as Facebook. For examples of <code>Logins</code> maps, see the code examples in the <a href=\\\"https://docs.aws.amazon.com/cognito/latest/developerguide/external-identity-providers.html\\\
  \">External Identity Providers</a> section of the Amazon Cognito Developer Guide.</p>\"\n        }\n      ]\n    },\n    \"CustomRoleArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ARNString\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the role to be assumed when multiple roles were received in the token from the identity provider. For example, a SAML-based identity provider. This parameter is optional for identity providers that do not support role customization.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"IdentityId\"\n  ],\n  \"description\": \"Input to the <code>GetCredentialsForIdentity</code> action.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-cognito/refs/heads/main/json-schema/cognito-identity-get-credentials-for-identity-input-schema.json\",\n  \"title\": \"GetCredentialsForIdentityInput\"\n\
  }"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-cognito/refs/heads/main/json-schema/cognito-identity-get-credentials-for-identity-input-schema.json
tags:
- Authentication
- Authorization
- Identity
- Identity Provider
- OAuth2
- OIDC
title: GetCredentialsForIdentityInput
---
