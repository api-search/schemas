---
description: AssociateResolverRuleRequest schema from openapi
layout: schema
name: AssociateResolverRuleRequest
properties_list:
- description: ''
  name: ResolverRuleId
  type: object
- description: ''
  name: Name
  type: object
- description: ''
  name: VPCId
  type: object
provider_name: Amazon Route 53 Resolver
provider_slug: amazon-route53-resolver
schema_file: json-schema/amazon-route53-resolver-openapi-associate-resolver-rule-request-schema.json
slug: amazon-route53-resolver-openapi-associate-resolver-rule-request
source_filename: amazon-route53-resolver-openapi-associate-resolver-rule-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-route53-resolver/refs/heads/main/json-schema/amazon-route53-resolver-openapi-associate-resolver-rule-request-schema.json\",\n  \"title\": \"AssociateResolverRuleRequest\",\n  \"description\": \"AssociateResolverRuleRequest schema from openapi\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ResolverRuleId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceId\"\n        },\n        {\n          \"description\": \"The ID of the Resolver rule that you want to associate with the VPC. To list the existing Resolver rules, use <a href=\\\"https://docs.aws.amazon.com/Route53/latest/APIReference/API_route53resolver_ListResolverRules.html\\\">ListResolverRules</a>.\"\n        }\n      ]\n    },\n    \"Name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Name\"\n        },\n\
  \        {\n          \"description\": \"A name for the association that you're creating between a Resolver rule and a VPC.\"\n        }\n      ]\n    },\n    \"VPCId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceId\"\n        },\n        {\n          \"description\": \"The ID of the VPC that you want to associate the Resolver rule with.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"ResolverRuleId\",\n    \"VPCId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-route53-resolver/refs/heads/main/json-schema/amazon-route53-resolver-openapi-associate-resolver-rule-request-schema.json
tags:
- AWS
- DNS
- Hybrid Cloud
- Networking
title: AssociateResolverRuleRequest
---
