---
description: DeleteFirewallRuleGroupRequest schema from openapi
layout: schema
name: DeleteFirewallRuleGroupRequest
properties_list:
- description: ''
  name: FirewallRuleGroupId
  type: object
provider_name: Amazon Route 53 Resolver
provider_slug: amazon-route53-resolver
schema_file: json-schema/amazon-route53-resolver-openapi-delete-firewall-rule-group-request-schema.json
slug: amazon-route53-resolver-openapi-delete-firewall-rule-group-request
source_filename: amazon-route53-resolver-openapi-delete-firewall-rule-group-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-route53-resolver/refs/heads/main/json-schema/amazon-route53-resolver-openapi-delete-firewall-rule-group-request-schema.json\",\n  \"title\": \"DeleteFirewallRuleGroupRequest\",\n  \"description\": \"DeleteFirewallRuleGroupRequest schema from openapi\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"FirewallRuleGroupId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceId\"\n        },\n        {\n          \"description\": \"The unique identifier of the firewall rule group that you want to delete. \"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"FirewallRuleGroupId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-route53-resolver/refs/heads/main/json-schema/amazon-route53-resolver-openapi-delete-firewall-rule-group-request-schema.json
tags:
- DNS
- Hybrid Cloud
- Networking
title: DeleteFirewallRuleGroupRequest
---
