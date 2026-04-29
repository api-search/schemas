---
description: In an <a href="https://docs.aws.amazon.com/Route53/latest/APIReference/API_route53resolver_UpdateResolverRule.html">UpdateResolverRule</a> request, information about the changes that you want to make.
layout: schema
name: ResolverRuleConfig
properties_list:
- description: ''
  name: Name
  type: object
- description: ''
  name: TargetIps
  type: object
- description: ''
  name: ResolverEndpointId
  type: object
provider_name: Amazon Route 53 Resolver
provider_slug: amazon-route53-resolver
schema_file: json-schema/amazon-route53-resolver-openapi-resolver-rule-config-schema.json
slug: amazon-route53-resolver-openapi-resolver-rule-config
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-route53-resolver/refs/heads/main/json-schema/amazon-route53-resolver-openapi-resolver-rule-config-schema.json\",\n  \"title\": \"ResolverRuleConfig\",\n  \"description\": \"In an <a href=\\\"https://docs.aws.amazon.com/Route53/latest/APIReference/API_route53resolver_UpdateResolverRule.html\\\">UpdateResolverRule</a> request, information about the changes that you want to make.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Name\"\n        },\n        {\n          \"description\": \"The new name for the Resolver rule. The name that you specify appears in the Resolver dashboard in the Route 53 console. \"\n        }\n      ]\n    },\n    \"TargetIps\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TargetList\"\n     \
  \   },\n        {\n          \"description\": \"For DNS queries that originate in your VPC, the new IP addresses that you want to route outbound DNS queries to.\"\n        }\n      ]\n    },\n    \"ResolverEndpointId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceId\"\n        },\n        {\n          \"description\": \"The ID of the new outbound Resolver endpoint that you want to use to route DNS queries to the IP addresses that you specify in <code>TargetIps</code>.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-route53-resolver/refs/heads/main/json-schema/amazon-route53-resolver-openapi-resolver-rule-config-schema.json
tags:
- AWS
- DNS
- Hybrid Cloud
- Networking
title: ResolverRuleConfig
---
