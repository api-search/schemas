---
description: DeleteUserPoolDomainRequest schema from Amazon Cognito API
layout: schema
name: DeleteUserPoolDomainRequest
properties_list:
- description: ''
  name: Domain
  type: object
- description: ''
  name: UserPoolId
  type: object
provider_name: Amazon Cognito
provider_slug: amazon-cognito
schema_file: json-schema/user-pools-delete-user-pool-domain-request-schema.json
slug: user-pools-delete-user-pool-domain-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-cognito/refs/heads/main/json-schema/user-pools-delete-user-pool-domain-request-schema.json\",\n  \"title\": \"DeleteUserPoolDomainRequest\",\n  \"description\": \"DeleteUserPoolDomainRequest schema from Amazon Cognito API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Domain\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DomainType\"\n        },\n        {\n          \"description\": \"The domain string. For custom domains, this is the fully-qualified domain name, such as <code>auth.example.com</code>. For Amazon Cognito prefix domains, this is the prefix alone, such as <code>auth</code>.\"\n        }\n      ]\n    },\n    \"UserPoolId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UserPoolIdType\"\n        },\n        {\n          \"description\": \"The user pool\
  \ ID.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Domain\",\n    \"UserPoolId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-cognito/refs/heads/main/json-schema/user-pools-delete-user-pool-domain-request-schema.json
tags:
- Authentication
- AWS
- Identity
- OAuth
- User Management
title: DeleteUserPoolDomainRequest
---
