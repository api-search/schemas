---
description: DisassociateResolverRuleResponse schema from openapi
layout: schema
name: DisassociateResolverRuleResponse
properties_list:
- description: ''
  name: ResolverRuleAssociation
  type: object
provider_name: Amazon Route 53 Resolver
provider_slug: amazon-route53-resolver
schema_file: json-schema/amazon-route53-resolver-openapi-disassociate-resolver-rule-response-schema.json
slug: amazon-route53-resolver-openapi-disassociate-resolver-rule-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-route53-resolver/refs/heads/main/json-schema/amazon-route53-resolver-openapi-disassociate-resolver-rule-response-schema.json\",\n  \"title\": \"DisassociateResolverRuleResponse\",\n  \"description\": \"DisassociateResolverRuleResponse schema from openapi\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ResolverRuleAssociation\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResolverRuleAssociation\"\n        },\n        {\n          \"description\": \"Information about the <code>DisassociateResolverRule</code> request, including the status of the request.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-route53-resolver/refs/heads/main/json-schema/amazon-route53-resolver-openapi-disassociate-resolver-rule-response-schema.json
tags:
- AWS
- DNS
- Hybrid Cloud
- Networking
title: DisassociateResolverRuleResponse
---
