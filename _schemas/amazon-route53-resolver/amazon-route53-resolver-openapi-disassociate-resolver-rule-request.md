---
description: DisassociateResolverRuleRequest schema from openapi
layout: schema
name: DisassociateResolverRuleRequest
properties_list:
- description: ''
  name: VPCId
  type: object
- description: ''
  name: ResolverRuleId
  type: object
provider_name: Amazon Route 53 Resolver
provider_slug: amazon-route53-resolver
schema_file: json-schema/amazon-route53-resolver-openapi-disassociate-resolver-rule-request-schema.json
slug: amazon-route53-resolver-openapi-disassociate-resolver-rule-request
source_filename: amazon-route53-resolver-openapi-disassociate-resolver-rule-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-route53-resolver/refs/heads/main/json-schema/amazon-route53-resolver-openapi-disassociate-resolver-rule-request-schema.json\",\n  \"title\": \"DisassociateResolverRuleRequest\",\n  \"description\": \"DisassociateResolverRuleRequest schema from openapi\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"VPCId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceId\"\n        },\n        {\n          \"description\": \"The ID of the VPC that you want to disassociate the Resolver rule from.\"\n        }\n      ]\n    },\n    \"ResolverRuleId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceId\"\n        },\n        {\n          \"description\": \"The ID of the Resolver rule that you want to disassociate from the specified VPC.\"\n        }\n      ]\n    }\n  },\n \
  \ \"required\": [\n    \"VPCId\",\n    \"ResolverRuleId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-route53-resolver/refs/heads/main/json-schema/amazon-route53-resolver-openapi-disassociate-resolver-rule-request-schema.json
tags:
- AWS
- DNS
- Hybrid Cloud
- Networking
title: DisassociateResolverRuleRequest
---
