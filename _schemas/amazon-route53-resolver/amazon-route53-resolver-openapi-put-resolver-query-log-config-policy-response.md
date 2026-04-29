---
description: The response to a <code>PutResolverQueryLogConfigPolicy</code> request.
layout: schema
name: PutResolverQueryLogConfigPolicyResponse
properties_list:
- description: ''
  name: ReturnValue
  type: object
provider_name: Amazon Route 53 Resolver
provider_slug: amazon-route53-resolver
schema_file: json-schema/amazon-route53-resolver-openapi-put-resolver-query-log-config-policy-response-schema.json
slug: amazon-route53-resolver-openapi-put-resolver-query-log-config-policy-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-route53-resolver/refs/heads/main/json-schema/amazon-route53-resolver-openapi-put-resolver-query-log-config-policy-response-schema.json\",\n  \"title\": \"PutResolverQueryLogConfigPolicyResponse\",\n  \"description\": \"The response to a <code>PutResolverQueryLogConfigPolicy</code> request.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ReturnValue\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Boolean\"\n        },\n        {\n          \"description\": \"Whether the <code>PutResolverQueryLogConfigPolicy</code> request was successful.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-route53-resolver/refs/heads/main/json-schema/amazon-route53-resolver-openapi-put-resolver-query-log-config-policy-response-schema.json
tags:
- AWS
- DNS
- Hybrid Cloud
- Networking
title: PutResolverQueryLogConfigPolicyResponse
---
