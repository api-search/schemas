---
description: The response to a <code>PutResolverRulePolicy</code> request.
layout: schema
name: PutResolverRulePolicyResponse
properties_list:
- description: ''
  name: ReturnValue
  type: object
provider_name: Amazon Route 53 Resolver
provider_slug: amazon-route53-resolver
schema_file: json-schema/amazon-route53-resolver-openapi-put-resolver-rule-policy-response-schema.json
slug: amazon-route53-resolver-openapi-put-resolver-rule-policy-response
source_filename: amazon-route53-resolver-openapi-put-resolver-rule-policy-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-route53-resolver/refs/heads/main/json-schema/amazon-route53-resolver-openapi-put-resolver-rule-policy-response-schema.json\",\n  \"title\": \"PutResolverRulePolicyResponse\",\n  \"description\": \"The response to a <code>PutResolverRulePolicy</code> request.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ReturnValue\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Boolean\"\n        },\n        {\n          \"description\": \"Whether the <code>PutResolverRulePolicy</code> request was successful.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-route53-resolver/refs/heads/main/json-schema/amazon-route53-resolver-openapi-put-resolver-rule-policy-response-schema.json
tags:
- DNS
- Hybrid Cloud
- Networking
title: PutResolverRulePolicyResponse
---
