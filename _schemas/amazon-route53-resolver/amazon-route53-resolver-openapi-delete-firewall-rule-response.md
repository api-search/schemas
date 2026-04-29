---
description: DeleteFirewallRuleResponse schema from openapi
layout: schema
name: DeleteFirewallRuleResponse
properties_list:
- description: ''
  name: FirewallRule
  type: object
provider_name: Amazon Route 53 Resolver
provider_slug: amazon-route53-resolver
schema_file: json-schema/amazon-route53-resolver-openapi-delete-firewall-rule-response-schema.json
slug: amazon-route53-resolver-openapi-delete-firewall-rule-response
source_filename: amazon-route53-resolver-openapi-delete-firewall-rule-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-route53-resolver/refs/heads/main/json-schema/amazon-route53-resolver-openapi-delete-firewall-rule-response-schema.json\",\n  \"title\": \"DeleteFirewallRuleResponse\",\n  \"description\": \"DeleteFirewallRuleResponse schema from openapi\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"FirewallRule\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FirewallRule\"\n        },\n        {\n          \"description\": \"The specification for the firewall rule that you just deleted.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-route53-resolver/refs/heads/main/json-schema/amazon-route53-resolver-openapi-delete-firewall-rule-response-schema.json
tags:
- AWS
- DNS
- Hybrid Cloud
- Networking
title: DeleteFirewallRuleResponse
---
