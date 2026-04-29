---
description: GetResolverQueryLogConfigPolicyRequest schema from openapi
layout: schema
name: GetResolverQueryLogConfigPolicyRequest
properties_list:
- description: ''
  name: Arn
  type: object
provider_name: Amazon Route 53 Resolver
provider_slug: amazon-route53-resolver
schema_file: json-schema/amazon-route53-resolver-openapi-get-resolver-query-log-config-policy-request-schema.json
slug: amazon-route53-resolver-openapi-get-resolver-query-log-config-policy-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-route53-resolver/refs/heads/main/json-schema/amazon-route53-resolver-openapi-get-resolver-query-log-config-policy-request-schema.json\",\n  \"title\": \"GetResolverQueryLogConfigPolicyRequest\",\n  \"description\": \"GetResolverQueryLogConfigPolicyRequest schema from openapi\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Arn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Arn\"\n        },\n        {\n          \"description\": \"The ARN of the query logging configuration that you want to get the query logging policy for.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Arn\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-route53-resolver/refs/heads/main/json-schema/amazon-route53-resolver-openapi-get-resolver-query-log-config-policy-request-schema.json
tags:
- AWS
- DNS
- Hybrid Cloud
- Networking
title: GetResolverQueryLogConfigPolicyRequest
---
