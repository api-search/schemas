---
description: CreateUserPoolDomainResponse schema from Amazon Cognito
layout: schema
name: CreateUserPoolDomainResponse
properties_list:
- description: ''
  name: CloudFrontDomain
  type: object
provider_name: Amazon Cognito
provider_slug: aws-cognito
schema_file: json-schema/cognito-idp-create-user-pool-domain-response-schema.json
slug: cognito-idp-create-user-pool-domain-response
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"CloudFrontDomain\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DomainType\"\n        },\n        {\n          \"description\": \"The Amazon CloudFront endpoint that you use as the target of the alias that you set up with your Domain Name Service (DNS) provider.\"\n        }\n      ]\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-cognito/refs/heads/main/json-schema/cognito-idp-create-user-pool-domain-response-schema.json\",\n  \"title\": \"CreateUserPoolDomainResponse\",\n  \"description\": \"CreateUserPoolDomainResponse schema from Amazon Cognito\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-cognito/refs/heads/main/json-schema/cognito-idp-create-user-pool-domain-response-schema.json
tags:
- Authentication
- Authorization
- AWS
- Identity
- Identity Provider
- OAuth2
- OIDC
title: CreateUserPoolDomainResponse
---
