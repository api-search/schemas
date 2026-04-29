---
description: The UpdateUserPoolDomain response output.
layout: schema
name: UpdateUserPoolDomainResponse
properties_list:
- description: ''
  name: CloudFrontDomain
  type: object
provider_name: Amazon Cognito
provider_slug: aws-cognito
schema_file: json-schema/cognito-idp-update-user-pool-domain-response-schema.json
slug: cognito-idp-update-user-pool-domain-response
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"CloudFrontDomain\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DomainType\"\n        },\n        {\n          \"description\": \"The Amazon CloudFront endpoint that Amazon Cognito set up when you added the custom domain to your user pool.\"\n        }\n      ]\n    }\n  },\n  \"description\": \"The UpdateUserPoolDomain response output.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-cognito/refs/heads/main/json-schema/cognito-idp-update-user-pool-domain-response-schema.json\",\n  \"title\": \"UpdateUserPoolDomainResponse\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-cognito/refs/heads/main/json-schema/cognito-idp-update-user-pool-domain-response-schema.json
tags:
- Authentication
- Authorization
- AWS
- Identity
- Identity Provider
- OAuth2
- OIDC
title: UpdateUserPoolDomainResponse
---
