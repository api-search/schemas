---
description: AssociateFirewallRuleGroupResponse schema from openapi
layout: schema
name: AssociateFirewallRuleGroupResponse
properties_list:
- description: ''
  name: FirewallRuleGroupAssociation
  type: object
provider_name: Amazon Route 53 Resolver
provider_slug: amazon-route53-resolver
schema_file: json-schema/amazon-route53-resolver-openapi-associate-firewall-rule-group-response-schema.json
slug: amazon-route53-resolver-openapi-associate-firewall-rule-group-response
source_filename: amazon-route53-resolver-openapi-associate-firewall-rule-group-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-route53-resolver/refs/heads/main/json-schema/amazon-route53-resolver-openapi-associate-firewall-rule-group-response-schema.json\",\n  \"title\": \"AssociateFirewallRuleGroupResponse\",\n  \"description\": \"AssociateFirewallRuleGroupResponse schema from openapi\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"FirewallRuleGroupAssociation\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FirewallRuleGroupAssociation\"\n        },\n        {\n          \"description\": \"The association that you just created. The association has an ID that you can use to identify it in other requests, like update and delete.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-route53-resolver/refs/heads/main/json-schema/amazon-route53-resolver-openapi-associate-firewall-rule-group-response-schema.json
tags:
- DNS
- Hybrid Cloud
- Networking
title: AssociateFirewallRuleGroupResponse
---
