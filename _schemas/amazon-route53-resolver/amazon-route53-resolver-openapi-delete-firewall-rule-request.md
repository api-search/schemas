---
description: DeleteFirewallRuleRequest schema from openapi
layout: schema
name: DeleteFirewallRuleRequest
properties_list:
- description: ''
  name: FirewallRuleGroupId
  type: object
- description: ''
  name: FirewallDomainListId
  type: object
provider_name: Amazon Route 53 Resolver
provider_slug: amazon-route53-resolver
schema_file: json-schema/amazon-route53-resolver-openapi-delete-firewall-rule-request-schema.json
slug: amazon-route53-resolver-openapi-delete-firewall-rule-request
source_filename: amazon-route53-resolver-openapi-delete-firewall-rule-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-route53-resolver/refs/heads/main/json-schema/amazon-route53-resolver-openapi-delete-firewall-rule-request-schema.json\",\n  \"title\": \"DeleteFirewallRuleRequest\",\n  \"description\": \"DeleteFirewallRuleRequest schema from openapi\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"FirewallRuleGroupId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceId\"\n        },\n        {\n          \"description\": \"The unique identifier of the firewall rule group that you want to delete the rule from. \"\n        }\n      ]\n    },\n    \"FirewallDomainListId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceId\"\n        },\n        {\n          \"description\": \"The ID of the domain list that's used in the rule. \"\n        }\n      ]\n    }\n  },\n  \"required\"\
  : [\n    \"FirewallRuleGroupId\",\n    \"FirewallDomainListId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-route53-resolver/refs/heads/main/json-schema/amazon-route53-resolver-openapi-delete-firewall-rule-request-schema.json
tags:
- DNS
- Hybrid Cloud
- Networking
title: DeleteFirewallRuleRequest
---
