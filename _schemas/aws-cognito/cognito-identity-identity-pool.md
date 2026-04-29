---
description: An object representing an Amazon Cognito identity pool.
layout: schema
name: IdentityPool
properties_list:
- description: ''
  name: IdentityPoolId
  type: object
- description: ''
  name: IdentityPoolName
  type: object
- description: ''
  name: AllowUnauthenticatedIdentities
  type: object
- description: ''
  name: AllowClassicFlow
  type: object
- description: ''
  name: SupportedLoginProviders
  type: object
- description: ''
  name: DeveloperProviderName
  type: object
- description: ''
  name: OpenIdConnectProviderARNs
  type: object
- description: ''
  name: CognitoIdentityProviders
  type: object
- description: ''
  name: SamlProviderARNs
  type: object
- description: ''
  name: IdentityPoolTags
  type: object
provider_name: Amazon Cognito
provider_slug: aws-cognito
schema_file: json-schema/cognito-identity-identity-pool-schema.json
slug: cognito-identity-identity-pool
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"IdentityPoolId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IdentityPoolId\"\n        },\n        {\n          \"description\": \"An identity pool ID in the format REGION:GUID.\"\n        }\n      ]\n    },\n    \"IdentityPoolName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IdentityPoolName\"\n        },\n        {\n          \"description\": \"A string that you provide.\"\n        }\n      ]\n    },\n    \"AllowUnauthenticatedIdentities\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IdentityPoolUnauthenticated\"\n        },\n        {\n          \"description\": \"TRUE if the identity pool supports unauthenticated logins.\"\n        }\n      ]\n    },\n    \"AllowClassicFlow\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ClassicFlow\"\n        },\n        {\n          \"description\"\
  : \"Enables or disables the Basic (Classic) authentication flow. For more information, see <a href=\\\"https://docs.aws.amazon.com/cognito/latest/developerguide/authentication-flow.html\\\">Identity Pools (Federated Identities) Authentication Flow</a> in the <i>Amazon Cognito Developer Guide</i>.\"\n        }\n      ]\n    },\n    \"SupportedLoginProviders\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IdentityProviders\"\n        },\n        {\n          \"description\": \"Optional key:value pairs mapping provider names to provider app IDs.\"\n        }\n      ]\n    },\n    \"DeveloperProviderName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DeveloperProviderName\"\n        },\n        {\n          \"description\": \"The \\\"domain\\\" by which Cognito will refer to your users.\"\n        }\n      ]\n    },\n    \"OpenIdConnectProviderARNs\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/OIDCProviderList\"\
  \n        },\n        {\n          \"description\": \"The ARNs of the OpenID Connect providers.\"\n        }\n      ]\n    },\n    \"CognitoIdentityProviders\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CognitoIdentityProviderList\"\n        },\n        {\n          \"description\": \"A list representing an Amazon Cognito user pool and its client ID.\"\n        }\n      ]\n    },\n    \"SamlProviderARNs\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SAMLProviderList\"\n        },\n        {\n          \"description\": \"An array of Amazon Resource Names (ARNs) of the SAML provider for your identity pool.\"\n        }\n      ]\n    },\n    \"IdentityPoolTags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IdentityPoolTagsType\"\n        },\n        {\n          \"description\": \"The tags that are assigned to the identity pool. A tag is a label that you can apply to identity pools to categorize\
  \ and manage them in different ways, such as by purpose, owner, environment, or other criteria.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"IdentityPoolId\",\n    \"IdentityPoolName\",\n    \"AllowUnauthenticatedIdentities\"\n  ],\n  \"description\": \"An object representing an Amazon Cognito identity pool.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-cognito/refs/heads/main/json-schema/cognito-identity-identity-pool-schema.json\",\n  \"title\": \"IdentityPool\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-cognito/refs/heads/main/json-schema/cognito-identity-identity-pool-schema.json
tags:
- Authentication
- Authorization
- AWS
- Identity
- Identity Provider
- OAuth2
- OIDC
title: IdentityPool
---
