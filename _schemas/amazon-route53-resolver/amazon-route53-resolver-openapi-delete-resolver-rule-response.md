---
description: DeleteResolverRuleResponse schema from openapi
layout: schema
name: DeleteResolverRuleResponse
properties_list:
- description: ''
  name: ResolverRule
  type: object
provider_name: Amazon Route 53 Resolver
provider_slug: amazon-route53-resolver
schema_file: json-schema/amazon-route53-resolver-openapi-delete-resolver-rule-response-schema.json
slug: amazon-route53-resolver-openapi-delete-resolver-rule-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-route53-resolver/refs/heads/main/json-schema/amazon-route53-resolver-openapi-delete-resolver-rule-response-schema.json\",\n  \"title\": \"DeleteResolverRuleResponse\",\n  \"description\": \"DeleteResolverRuleResponse schema from openapi\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ResolverRule\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResolverRule\"\n        },\n        {\n          \"description\": \"Information about the <code>DeleteResolverRule</code> request, including the status of the request.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-route53-resolver/refs/heads/main/json-schema/amazon-route53-resolver-openapi-delete-resolver-rule-response-schema.json
tags:
- AWS
- DNS
- Hybrid Cloud
- Networking
title: DeleteResolverRuleResponse
---
