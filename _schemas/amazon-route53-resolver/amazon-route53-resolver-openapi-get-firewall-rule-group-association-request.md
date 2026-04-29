---
description: GetFirewallRuleGroupAssociationRequest schema from openapi
layout: schema
name: GetFirewallRuleGroupAssociationRequest
properties_list:
- description: ''
  name: FirewallRuleGroupAssociationId
  type: object
provider_name: Amazon Route 53 Resolver
provider_slug: amazon-route53-resolver
schema_file: json-schema/amazon-route53-resolver-openapi-get-firewall-rule-group-association-request-schema.json
slug: amazon-route53-resolver-openapi-get-firewall-rule-group-association-request
source_filename: amazon-route53-resolver-openapi-get-firewall-rule-group-association-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-route53-resolver/refs/heads/main/json-schema/amazon-route53-resolver-openapi-get-firewall-rule-group-association-request-schema.json\",\n  \"title\": \"GetFirewallRuleGroupAssociationRequest\",\n  \"description\": \"GetFirewallRuleGroupAssociationRequest schema from openapi\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"FirewallRuleGroupAssociationId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceId\"\n        },\n        {\n          \"description\": \"The identifier of the <a>FirewallRuleGroupAssociation</a>. \"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"FirewallRuleGroupAssociationId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-route53-resolver/refs/heads/main/json-schema/amazon-route53-resolver-openapi-get-firewall-rule-group-association-request-schema.json
tags:
- AWS
- DNS
- Hybrid Cloud
- Networking
title: GetFirewallRuleGroupAssociationRequest
---
