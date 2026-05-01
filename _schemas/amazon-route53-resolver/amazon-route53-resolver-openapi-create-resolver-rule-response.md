---
description: CreateResolverRuleResponse schema from openapi
layout: schema
name: CreateResolverRuleResponse
properties_list:
- description: ''
  name: ResolverRule
  type: object
provider_name: Amazon Route 53 Resolver
provider_slug: amazon-route53-resolver
schema_file: json-schema/amazon-route53-resolver-openapi-create-resolver-rule-response-schema.json
slug: amazon-route53-resolver-openapi-create-resolver-rule-response
source_filename: amazon-route53-resolver-openapi-create-resolver-rule-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-route53-resolver/refs/heads/main/json-schema/amazon-route53-resolver-openapi-create-resolver-rule-response-schema.json\",\n  \"title\": \"CreateResolverRuleResponse\",\n  \"description\": \"CreateResolverRuleResponse schema from openapi\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ResolverRule\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResolverRule\"\n        },\n        {\n          \"description\": \"Information about the <code>CreateResolverRule</code> request, including the status of the request.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-route53-resolver/refs/heads/main/json-schema/amazon-route53-resolver-openapi-create-resolver-rule-response-schema.json
tags:
- DNS
- Hybrid Cloud
- Networking
title: CreateResolverRuleResponse
---
