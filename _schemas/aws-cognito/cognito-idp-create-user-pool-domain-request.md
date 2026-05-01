---
description: CreateUserPoolDomainRequest schema from Amazon Cognito
layout: schema
name: CreateUserPoolDomainRequest
properties_list:
- description: ''
  name: Domain
  type: object
- description: ''
  name: UserPoolId
  type: object
- description: ''
  name: CustomDomainConfig
  type: object
provider_name: Amazon Cognito
provider_slug: aws-cognito
schema_file: json-schema/cognito-idp-create-user-pool-domain-request-schema.json
slug: cognito-idp-create-user-pool-domain-request
source_filename: cognito-idp-create-user-pool-domain-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"Domain\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DomainType\"\n        },\n        {\n          \"description\": \"The domain string. For custom domains, this is the fully-qualified domain name, such as <code>auth.example.com</code>. For Amazon Cognito prefix domains, this is the prefix alone, such as <code>auth</code>.\"\n        }\n      ]\n    },\n    \"UserPoolId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UserPoolIdType\"\n        },\n        {\n          \"description\": \"The user pool ID.\"\n        }\n      ]\n    },\n    \"CustomDomainConfig\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CustomDomainConfigType\"\n        },\n        {\n          \"description\": \"<p>The configuration for a custom domain that hosts the sign-up and sign-in webpages for your application.</p> <p>Provide this parameter only if\
  \ you want to use a custom domain for your user pool. Otherwise, you can exclude this parameter and use the Amazon Cognito hosted domain instead.</p> <p>For more information about the hosted domain and custom domains, see <a href=\\\"https://docs.aws.amazon.com/cognito/latest/developerguide/cognito-user-pools-assign-domain.html\\\">Configuring a User Pool Domain</a>.</p>\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Domain\",\n    \"UserPoolId\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-cognito/refs/heads/main/json-schema/cognito-idp-create-user-pool-domain-request-schema.json\",\n  \"title\": \"CreateUserPoolDomainRequest\",\n  \"description\": \"CreateUserPoolDomainRequest schema from Amazon Cognito\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-cognito/refs/heads/main/json-schema/cognito-idp-create-user-pool-domain-request-schema.json
tags:
- Authentication
- Authorization
- Identity
- Identity Provider
- OAuth2
- OIDC
title: CreateUserPoolDomainRequest
---
