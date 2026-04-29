---
description: CreateFirewallRuleGroupResponse schema from openapi
layout: schema
name: CreateFirewallRuleGroupResponse
properties_list:
- description: ''
  name: FirewallRuleGroup
  type: object
provider_name: Amazon Route 53 Resolver
provider_slug: amazon-route53-resolver
schema_file: json-schema/amazon-route53-resolver-openapi-create-firewall-rule-group-response-schema.json
slug: amazon-route53-resolver-openapi-create-firewall-rule-group-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-route53-resolver/refs/heads/main/json-schema/amazon-route53-resolver-openapi-create-firewall-rule-group-response-schema.json\",\n  \"title\": \"CreateFirewallRuleGroupResponse\",\n  \"description\": \"CreateFirewallRuleGroupResponse schema from openapi\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"FirewallRuleGroup\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FirewallRuleGroup\"\n        },\n        {\n          \"description\": \"A collection of rules used to filter DNS network traffic. \"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-route53-resolver/refs/heads/main/json-schema/amazon-route53-resolver-openapi-create-firewall-rule-group-response-schema.json
tags:
- AWS
- DNS
- Hybrid Cloud
- Networking
title: CreateFirewallRuleGroupResponse
---
