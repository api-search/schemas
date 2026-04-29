---
description: DisassociateFirewallRuleGroupRequest schema from openapi
layout: schema
name: DisassociateFirewallRuleGroupRequest
properties_list:
- description: ''
  name: FirewallRuleGroupAssociationId
  type: object
provider_name: Amazon Route 53 Resolver
provider_slug: amazon-route53-resolver
schema_file: json-schema/amazon-route53-resolver-openapi-disassociate-firewall-rule-group-request-schema.json
slug: amazon-route53-resolver-openapi-disassociate-firewall-rule-group-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-route53-resolver/refs/heads/main/json-schema/amazon-route53-resolver-openapi-disassociate-firewall-rule-group-request-schema.json\",\n  \"title\": \"DisassociateFirewallRuleGroupRequest\",\n  \"description\": \"DisassociateFirewallRuleGroupRequest schema from openapi\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"FirewallRuleGroupAssociationId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceId\"\n        },\n        {\n          \"description\": \"The identifier of the <a>FirewallRuleGroupAssociation</a>. \"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"FirewallRuleGroupAssociationId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-route53-resolver/refs/heads/main/json-schema/amazon-route53-resolver-openapi-disassociate-firewall-rule-group-request-schema.json
tags:
- AWS
- DNS
- Hybrid Cloud
- Networking
title: DisassociateFirewallRuleGroupRequest
---
