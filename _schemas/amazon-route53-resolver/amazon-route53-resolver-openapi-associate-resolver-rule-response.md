---
description: AssociateResolverRuleResponse schema from openapi
layout: schema
name: AssociateResolverRuleResponse
properties_list:
- description: ''
  name: ResolverRuleAssociation
  type: object
provider_name: Amazon Route 53 Resolver
provider_slug: amazon-route53-resolver
schema_file: json-schema/amazon-route53-resolver-openapi-associate-resolver-rule-response-schema.json
slug: amazon-route53-resolver-openapi-associate-resolver-rule-response
source_filename: amazon-route53-resolver-openapi-associate-resolver-rule-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-route53-resolver/refs/heads/main/json-schema/amazon-route53-resolver-openapi-associate-resolver-rule-response-schema.json\",\n  \"title\": \"AssociateResolverRuleResponse\",\n  \"description\": \"AssociateResolverRuleResponse schema from openapi\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ResolverRuleAssociation\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResolverRuleAssociation\"\n        },\n        {\n          \"description\": \"Information about the <code>AssociateResolverRule</code> request, including the status of the request.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-route53-resolver/refs/heads/main/json-schema/amazon-route53-resolver-openapi-associate-resolver-rule-response-schema.json
tags:
- DNS
- Hybrid Cloud
- Networking
title: AssociateResolverRuleResponse
---
