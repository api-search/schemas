---
description: CreateUserPoolDomainResponse schema from Amazon Cognito API
layout: schema
name: CreateUserPoolDomainResponse
properties_list:
- description: ''
  name: CloudFrontDomain
  type: object
provider_name: Amazon Cognito
provider_slug: amazon-cognito
schema_file: json-schema/user-pools-create-user-pool-domain-response-schema.json
slug: user-pools-create-user-pool-domain-response
source_filename: user-pools-create-user-pool-domain-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-cognito/refs/heads/main/json-schema/user-pools-create-user-pool-domain-response-schema.json\",\n  \"title\": \"CreateUserPoolDomainResponse\",\n  \"description\": \"CreateUserPoolDomainResponse schema from Amazon Cognito API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"CloudFrontDomain\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DomainType\"\n        },\n        {\n          \"description\": \"The Amazon CloudFront endpoint that you use as the target of the alias that you set up with your Domain Name Service (DNS) provider.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-cognito/refs/heads/main/json-schema/user-pools-create-user-pool-domain-response-schema.json
tags:
- Authentication
- Identity
- OAuth
- User Management
title: CreateUserPoolDomainResponse
---
