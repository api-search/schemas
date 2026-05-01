---
description: DescribeUserPoolDomainRequest schema from Amazon Cognito API
layout: schema
name: DescribeUserPoolDomainRequest
properties_list:
- description: ''
  name: Domain
  type: object
provider_name: Amazon Cognito
provider_slug: amazon-cognito
schema_file: json-schema/user-pools-describe-user-pool-domain-request-schema.json
slug: user-pools-describe-user-pool-domain-request
source_filename: user-pools-describe-user-pool-domain-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-cognito/refs/heads/main/json-schema/user-pools-describe-user-pool-domain-request-schema.json\",\n  \"title\": \"DescribeUserPoolDomainRequest\",\n  \"description\": \"DescribeUserPoolDomainRequest schema from Amazon Cognito API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Domain\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DomainType\"\n        },\n        {\n          \"description\": \"The domain string. For custom domains, this is the fully-qualified domain name, such as <code>auth.example.com</code>. For Amazon Cognito prefix domains, this is the prefix alone, such as <code>auth</code>.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Domain\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-cognito/refs/heads/main/json-schema/user-pools-describe-user-pool-domain-request-schema.json
tags:
- Authentication
- Identity
- OAuth
- User Management
title: DescribeUserPoolDomainRequest
---
