---
description: UpdateFirewallPolicyResponse schema from Amazon Network Firewall
layout: schema
name: UpdateFirewallPolicyResponse
properties_list:
- description: ''
  name: UpdateToken
  type: object
- description: ''
  name: FirewallPolicyResponse
  type: object
provider_name: Amazon Network Firewall
provider_slug: amazon-network-firewall
schema_file: json-schema/openapi-update-firewall-policy-response-schema.json
slug: openapi-update-firewall-policy-response
source_filename: openapi-update-firewall-policy-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-network-firewall/refs/heads/main/json-schema/openapi-update-firewall-policy-response-schema.json\",\n  \"title\": \"UpdateFirewallPolicyResponse\",\n  \"description\": \"UpdateFirewallPolicyResponse schema from Amazon Network Firewall\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"UpdateToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UpdateToken\"\n        },\n        {\n          \"description\": \"<p>A token used for optimistic locking. Network Firewall returns a token to your requests that access the firewall policy. The token marks the state of the policy resource at the time of the request. </p> <p>To make changes to the policy, you provide the token in your request. Network Firewall uses the token to ensure that the policy hasn't changed since you last retrieved it. If it has changed, the\
  \ operation fails with an <code>InvalidTokenException</code>. If this happens, retrieve the firewall policy again to get a current copy of it with current token. Reapply your changes as needed, then try the operation again using the new token. </p>\"\n        }\n      ]\n    },\n    \"FirewallPolicyResponse\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FirewallPolicyResponse\"\n        },\n        {\n          \"description\": \"The high-level properties of a firewall policy. This, along with the <a>FirewallPolicy</a>, define the policy. You can retrieve all objects for a firewall policy by calling <a>DescribeFirewallPolicy</a>. \"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"UpdateToken\",\n    \"FirewallPolicyResponse\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-network-firewall/refs/heads/main/json-schema/openapi-update-firewall-policy-response-schema.json
tags:
- Firewall
- Intrusion Detection
- Network Security
- VPC
title: UpdateFirewallPolicyResponse
---
