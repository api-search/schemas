---
description: DeleteFirewallPolicyResponse schema from Amazon Network Firewall
layout: schema
name: DeleteFirewallPolicyResponse
properties_list:
- description: ''
  name: FirewallPolicyResponse
  type: object
provider_name: Amazon Network Firewall
provider_slug: amazon-network-firewall
schema_file: json-schema/openapi-delete-firewall-policy-response-schema.json
slug: openapi-delete-firewall-policy-response
source_filename: openapi-delete-firewall-policy-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-network-firewall/refs/heads/main/json-schema/openapi-delete-firewall-policy-response-schema.json\",\n  \"title\": \"DeleteFirewallPolicyResponse\",\n  \"description\": \"DeleteFirewallPolicyResponse schema from Amazon Network Firewall\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"FirewallPolicyResponse\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FirewallPolicyResponse\"\n        },\n        {\n          \"description\": \"The object containing the definition of the <a>FirewallPolicyResponse</a> that you asked to delete. \"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"FirewallPolicyResponse\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-network-firewall/refs/heads/main/json-schema/openapi-delete-firewall-policy-response-schema.json
tags:
- Firewall
- Intrusion Detection
- Network Security
- VPC
title: DeleteFirewallPolicyResponse
---
