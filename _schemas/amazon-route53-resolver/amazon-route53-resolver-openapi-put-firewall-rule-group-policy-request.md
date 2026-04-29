---
description: PutFirewallRuleGroupPolicyRequest schema from openapi
layout: schema
name: PutFirewallRuleGroupPolicyRequest
properties_list:
- description: ''
  name: Arn
  type: object
- description: ''
  name: FirewallRuleGroupPolicy
  type: object
provider_name: Amazon Route 53 Resolver
provider_slug: amazon-route53-resolver
schema_file: json-schema/amazon-route53-resolver-openapi-put-firewall-rule-group-policy-request-schema.json
slug: amazon-route53-resolver-openapi-put-firewall-rule-group-policy-request
source_filename: amazon-route53-resolver-openapi-put-firewall-rule-group-policy-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-route53-resolver/refs/heads/main/json-schema/amazon-route53-resolver-openapi-put-firewall-rule-group-policy-request-schema.json\",\n  \"title\": \"PutFirewallRuleGroupPolicyRequest\",\n  \"description\": \"PutFirewallRuleGroupPolicyRequest schema from openapi\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Arn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Arn\"\n        },\n        {\n          \"description\": \"The ARN (Amazon Resource Name) for the rule group that you want to share.\"\n        }\n      ]\n    },\n    \"FirewallRuleGroupPolicy\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FirewallRuleGroupPolicy\"\n        },\n        {\n          \"description\": \"The Identity and Access Management (Amazon Web Services IAM) policy to attach to the rule group.\"\
  \n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Arn\",\n    \"FirewallRuleGroupPolicy\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-route53-resolver/refs/heads/main/json-schema/amazon-route53-resolver-openapi-put-firewall-rule-group-policy-request-schema.json
tags:
- AWS
- DNS
- Hybrid Cloud
- Networking
title: PutFirewallRuleGroupPolicyRequest
---
