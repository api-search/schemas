---
description: The UpdateUserPoolDomain request input.
layout: schema
name: UpdateUserPoolDomainRequest
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
provider_slug: amazon-cognito
schema_file: json-schema/user-pools-update-user-pool-domain-request-schema.json
slug: user-pools-update-user-pool-domain-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-cognito/refs/heads/main/json-schema/user-pools-update-user-pool-domain-request-schema.json\",\n  \"title\": \"UpdateUserPoolDomainRequest\",\n  \"description\": \"The UpdateUserPoolDomain request input.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Domain\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DomainType\"\n        },\n        {\n          \"description\": \"<p>The domain name for the custom domain that hosts the sign-up and sign-in pages for your application. One example might be <code>auth.example.com</code>. </p> <p>This string can include only lowercase letters, numbers, and hyphens. Don't use a hyphen for the first or last character. Use periods to separate subdomain names.</p>\"\n        }\n      ]\n    },\n    \"UserPoolId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"\
  #/components/schemas/UserPoolIdType\"\n        },\n        {\n          \"description\": \"The ID of the user pool that is associated with the custom domain whose certificate you're updating.\"\n        }\n      ]\n    },\n    \"CustomDomainConfig\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CustomDomainConfigType\"\n        },\n        {\n          \"description\": \"The configuration for a custom domain that hosts the sign-up and sign-in pages for your application. Use this object to specify an SSL certificate that is managed by ACM.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Domain\",\n    \"UserPoolId\",\n    \"CustomDomainConfig\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-cognito/refs/heads/main/json-schema/user-pools-update-user-pool-domain-request-schema.json
tags:
- Authentication
- AWS
- Identity
- OAuth
- User Management
title: UpdateUserPoolDomainRequest
---
