---
description: GetFirewallRuleGroupPolicyResponse schema from openapi
layout: schema
name: GetFirewallRuleGroupPolicyResponse
properties_list:
- description: ''
  name: FirewallRuleGroupPolicy
  type: object
provider_name: Amazon Route 53 Resolver
provider_slug: amazon-route53-resolver
schema_file: json-schema/amazon-route53-resolver-openapi-get-firewall-rule-group-policy-response-schema.json
slug: amazon-route53-resolver-openapi-get-firewall-rule-group-policy-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-route53-resolver/refs/heads/main/json-schema/amazon-route53-resolver-openapi-get-firewall-rule-group-policy-response-schema.json\",\n  \"title\": \"GetFirewallRuleGroupPolicyResponse\",\n  \"description\": \"GetFirewallRuleGroupPolicyResponse schema from openapi\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"FirewallRuleGroupPolicy\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FirewallRuleGroupPolicy\"\n        },\n        {\n          \"description\": \"The Identity and Access Management (Amazon Web Services IAM) policy for sharing the specified rule group. You can use the policy to share the rule group using Resource Access Manager (RAM). \"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-route53-resolver/refs/heads/main/json-schema/amazon-route53-resolver-openapi-get-firewall-rule-group-policy-response-schema.json
tags:
- AWS
- DNS
- Hybrid Cloud
- Networking
title: GetFirewallRuleGroupPolicyResponse
---
