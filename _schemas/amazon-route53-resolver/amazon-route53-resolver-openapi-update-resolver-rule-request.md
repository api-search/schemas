---
description: UpdateResolverRuleRequest schema from openapi
layout: schema
name: UpdateResolverRuleRequest
properties_list:
- description: ''
  name: ResolverRuleId
  type: object
- description: ''
  name: Config
  type: object
provider_name: Amazon Route 53 Resolver
provider_slug: amazon-route53-resolver
schema_file: json-schema/amazon-route53-resolver-openapi-update-resolver-rule-request-schema.json
slug: amazon-route53-resolver-openapi-update-resolver-rule-request
source_filename: amazon-route53-resolver-openapi-update-resolver-rule-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-route53-resolver/refs/heads/main/json-schema/amazon-route53-resolver-openapi-update-resolver-rule-request-schema.json\",\n  \"title\": \"UpdateResolverRuleRequest\",\n  \"description\": \"UpdateResolverRuleRequest schema from openapi\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ResolverRuleId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceId\"\n        },\n        {\n          \"description\": \"The ID of the Resolver rule that you want to update.\"\n        }\n      ]\n    },\n    \"Config\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResolverRuleConfig\"\n        },\n        {\n          \"description\": \"The new settings for the Resolver rule.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"ResolverRuleId\",\n    \"Config\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-route53-resolver/refs/heads/main/json-schema/amazon-route53-resolver-openapi-update-resolver-rule-request-schema.json
tags:
- DNS
- Hybrid Cloud
- Networking
title: UpdateResolverRuleRequest
---
