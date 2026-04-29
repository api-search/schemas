---
description: CreateIdentityProviderRequest schema from Amazon Cognito
layout: schema
name: CreateIdentityProviderRequest
properties_list:
- description: ''
  name: UserPoolId
  type: object
- description: ''
  name: ProviderName
  type: object
- description: ''
  name: ProviderType
  type: object
- description: ''
  name: ProviderDetails
  type: object
- description: ''
  name: AttributeMapping
  type: object
- description: ''
  name: IdpIdentifiers
  type: object
provider_name: Amazon Cognito
provider_slug: aws-cognito
schema_file: json-schema/cognito-idp-create-identity-provider-request-schema.json
slug: cognito-idp-create-identity-provider-request
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"UserPoolId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UserPoolIdType\"\n        },\n        {\n          \"description\": \"The user pool ID.\"\n        }\n      ]\n    },\n    \"ProviderName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ProviderNameTypeV1\"\n        },\n        {\n          \"description\": \"The IdP name.\"\n        }\n      ]\n    },\n    \"ProviderType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IdentityProviderTypeType\"\n        },\n        {\n          \"description\": \"The IdP type.\"\n        }\n      ]\n    },\n    \"ProviderDetails\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ProviderDetailsType\"\n        },\n        {\n          \"description\": \"<p>The IdP details. The following list describes the provider detail keys for each IdP type.</p> <ul> <li>\
  \ <p>For Google and Login with Amazon:</p> <ul> <li> <p>client_id</p> </li> <li> <p>client_secret</p> </li> <li> <p>authorize_scopes</p> </li> </ul> </li> <li> <p>For Facebook:</p> <ul> <li> <p>client_id</p> </li> <li> <p>client_secret</p> </li> <li> <p>authorize_scopes</p> </li> <li> <p>api_version</p> </li> </ul> </li> <li> <p>For Sign in with Apple:</p> <ul> <li> <p>client_id</p> </li> <li> <p>team_id</p> </li> <li> <p>key_id</p> </li> <li> <p>private_key</p> </li> <li> <p>authorize_scopes</p> </li> </ul> </li> <li> <p>For OpenID Connect (OIDC) providers:</p> <ul> <li> <p>client_id</p> </li> <li> <p>client_secret</p> </li> <li> <p>attributes_request_method</p> </li> <li> <p>oidc_issuer</p> </li> <li> <p>authorize_scopes</p> </li> <li> <p>The following keys are only present if Amazon Cognito didn't discover them at the <code>oidc_issuer</code> URL.</p> <ul> <li> <p>authorize_url </p> </li> <li> <p>token_url </p> </li> <li> <p>attributes_url </p> </li> <li> <p>jwks_uri </p> </li> </ul>\
  \ </li> <li> <p>Amazon Cognito sets the value of the following keys automatically. They are read-only.</p> <ul> <li> <p>attributes_url_add_attributes </p> </li> </ul> </li> </ul> </li> <li> <p>For SAML providers:</p> <ul> <li> <p>MetadataFile or MetadataURL</p> </li> <li> <p>IDPSignout <i>optional</i> </p> </li> </ul> </li> </ul>\"\n        }\n      ]\n    },\n    \"AttributeMapping\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AttributeMappingType\"\n        },\n        {\n          \"description\": \"A mapping of IdP attributes to standard and custom user pool attributes.\"\n        }\n      ]\n    },\n    \"IdpIdentifiers\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IdpIdentifiersListType\"\n        },\n        {\n          \"description\": \"A list of IdP identifiers.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"UserPoolId\",\n    \"ProviderName\",\n    \"ProviderType\",\n    \"ProviderDetails\"\n\
  \  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-cognito/refs/heads/main/json-schema/cognito-idp-create-identity-provider-request-schema.json\",\n  \"title\": \"CreateIdentityProviderRequest\",\n  \"description\": \"CreateIdentityProviderRequest schema from Amazon Cognito\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-cognito/refs/heads/main/json-schema/cognito-idp-create-identity-provider-request-schema.json
tags:
- Authentication
- Authorization
- AWS
- Identity
- Identity Provider
- OAuth2
- OIDC
title: CreateIdentityProviderRequest
---
