---
description: GetResolverRulePolicyRequest schema from openapi
layout: schema
name: GetResolverRulePolicyRequest
properties_list:
- description: ''
  name: Arn
  type: object
provider_name: Amazon Route 53 Resolver
provider_slug: amazon-route53-resolver
schema_file: json-schema/amazon-route53-resolver-openapi-get-resolver-rule-policy-request-schema.json
slug: amazon-route53-resolver-openapi-get-resolver-rule-policy-request
source_filename: amazon-route53-resolver-openapi-get-resolver-rule-policy-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-route53-resolver/refs/heads/main/json-schema/amazon-route53-resolver-openapi-get-resolver-rule-policy-request-schema.json\",\n  \"title\": \"GetResolverRulePolicyRequest\",\n  \"description\": \"GetResolverRulePolicyRequest schema from openapi\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Arn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Arn\"\n        },\n        {\n          \"description\": \"The ID of the Resolver rule that you want to get the Resolver rule policy for.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Arn\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-route53-resolver/refs/heads/main/json-schema/amazon-route53-resolver-openapi-get-resolver-rule-policy-request-schema.json
tags:
- AWS
- DNS
- Hybrid Cloud
- Networking
title: GetResolverRulePolicyRequest
---
