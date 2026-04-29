---
description: DisassociateFirewallRuleGroupResponse schema from openapi
layout: schema
name: DisassociateFirewallRuleGroupResponse
properties_list:
- description: ''
  name: FirewallRuleGroupAssociation
  type: object
provider_name: Amazon Route 53 Resolver
provider_slug: amazon-route53-resolver
schema_file: json-schema/amazon-route53-resolver-openapi-disassociate-firewall-rule-group-response-schema.json
slug: amazon-route53-resolver-openapi-disassociate-firewall-rule-group-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-route53-resolver/refs/heads/main/json-schema/amazon-route53-resolver-openapi-disassociate-firewall-rule-group-response-schema.json\",\n  \"title\": \"DisassociateFirewallRuleGroupResponse\",\n  \"description\": \"DisassociateFirewallRuleGroupResponse schema from openapi\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"FirewallRuleGroupAssociation\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FirewallRuleGroupAssociation\"\n        },\n        {\n          \"description\": \"The firewall rule group association that you just removed. \"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-route53-resolver/refs/heads/main/json-schema/amazon-route53-resolver-openapi-disassociate-firewall-rule-group-response-schema.json
tags:
- AWS
- DNS
- Hybrid Cloud
- Networking
title: DisassociateFirewallRuleGroupResponse
---
