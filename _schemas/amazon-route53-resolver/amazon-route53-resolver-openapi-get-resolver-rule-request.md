---
description: GetResolverRuleRequest schema from openapi
layout: schema
name: GetResolverRuleRequest
properties_list:
- description: ''
  name: ResolverRuleId
  type: object
provider_name: Amazon Route 53 Resolver
provider_slug: amazon-route53-resolver
schema_file: json-schema/amazon-route53-resolver-openapi-get-resolver-rule-request-schema.json
slug: amazon-route53-resolver-openapi-get-resolver-rule-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-route53-resolver/refs/heads/main/json-schema/amazon-route53-resolver-openapi-get-resolver-rule-request-schema.json\",\n  \"title\": \"GetResolverRuleRequest\",\n  \"description\": \"GetResolverRuleRequest schema from openapi\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ResolverRuleId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceId\"\n        },\n        {\n          \"description\": \"The ID of the Resolver rule that you want to get information about.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"ResolverRuleId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-route53-resolver/refs/heads/main/json-schema/amazon-route53-resolver-openapi-get-resolver-rule-request-schema.json
tags:
- AWS
- DNS
- Hybrid Cloud
- Networking
title: GetResolverRuleRequest
---
