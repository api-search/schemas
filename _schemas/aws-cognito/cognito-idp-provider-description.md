---
description: A container for IdP details.
layout: schema
name: ProviderDescription
properties_list:
- description: ''
  name: ProviderName
  type: object
- description: ''
  name: ProviderType
  type: object
- description: ''
  name: LastModifiedDate
  type: object
- description: ''
  name: CreationDate
  type: object
provider_name: Amazon Cognito
provider_slug: aws-cognito
schema_file: json-schema/cognito-idp-provider-description-schema.json
slug: cognito-idp-provider-description
source_filename: cognito-idp-provider-description-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"ProviderName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ProviderNameType\"\n        },\n        {\n          \"description\": \"The IdP name.\"\n        }\n      ]\n    },\n    \"ProviderType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IdentityProviderTypeType\"\n        },\n        {\n          \"description\": \"The IdP type.\"\n        }\n      ]\n    },\n    \"LastModifiedDate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DateType\"\n        },\n        {\n          \"description\": \"The date the provider was last modified.\"\n        }\n      ]\n    },\n    \"CreationDate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DateType\"\n        },\n        {\n          \"description\": \"The date the provider was added to the user pool.\"\n        }\n      ]\n    }\n  },\n  \"description\"\
  : \"A container for IdP details.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-cognito/refs/heads/main/json-schema/cognito-idp-provider-description-schema.json\",\n  \"title\": \"ProviderDescription\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-cognito/refs/heads/main/json-schema/cognito-idp-provider-description-schema.json
tags:
- Authentication
- Authorization
- AWS
- Identity
- Identity Provider
- OAuth2
- OIDC
title: ProviderDescription
---
