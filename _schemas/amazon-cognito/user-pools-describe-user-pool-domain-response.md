---
description: DescribeUserPoolDomainResponse schema from Amazon Cognito API
layout: schema
name: DescribeUserPoolDomainResponse
properties_list:
- description: ''
  name: DomainDescription
  type: object
provider_name: Amazon Cognito
provider_slug: amazon-cognito
schema_file: json-schema/user-pools-describe-user-pool-domain-response-schema.json
slug: user-pools-describe-user-pool-domain-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-cognito/refs/heads/main/json-schema/user-pools-describe-user-pool-domain-response-schema.json\",\n  \"title\": \"DescribeUserPoolDomainResponse\",\n  \"description\": \"DescribeUserPoolDomainResponse schema from Amazon Cognito API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"DomainDescription\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DomainDescriptionType\"\n        },\n        {\n          \"description\": \"A domain description object containing information about the domain.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-cognito/refs/heads/main/json-schema/user-pools-describe-user-pool-domain-response-schema.json
tags:
- Authentication
- AWS
- Identity
- OAuth
- User Management
title: DescribeUserPoolDomainResponse
---
