---
description: A container for information about an IdP for a user pool.
layout: schema
name: ProviderUserIdentifierType
properties_list:
- description: ''
  name: ProviderName
  type: object
- description: ''
  name: ProviderAttributeName
  type: object
- description: ''
  name: ProviderAttributeValue
  type: object
provider_name: Amazon Cognito
provider_slug: aws-cognito
schema_file: json-schema/cognito-idp-provider-user-identifier-type-schema.json
slug: cognito-idp-provider-user-identifier-type
source_filename: cognito-idp-provider-user-identifier-type-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"ProviderName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ProviderNameType\"\n        },\n        {\n          \"description\": \"The name of the provider, such as Facebook, Google, or Login with Amazon.\"\n        }\n      ]\n    },\n    \"ProviderAttributeName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StringType\"\n        },\n        {\n          \"description\": \"The name of the provider attribute to link to, such as <code>NameID</code>.\"\n        }\n      ]\n    },\n    \"ProviderAttributeValue\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StringType\"\n        },\n        {\n          \"description\": \"The value of the provider attribute to link to, such as <code>xxxxx_account</code>.\"\n        }\n      ]\n    }\n  },\n  \"description\": \"A container for information about an IdP for a user pool.\",\n  \"\
  $schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-cognito/refs/heads/main/json-schema/cognito-idp-provider-user-identifier-type-schema.json\",\n  \"title\": \"ProviderUserIdentifierType\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-cognito/refs/heads/main/json-schema/cognito-idp-provider-user-identifier-type-schema.json
tags:
- Authentication
- Authorization
- AWS
- Identity
- Identity Provider
- OAuth2
- OIDC
title: ProviderUserIdentifierType
---
