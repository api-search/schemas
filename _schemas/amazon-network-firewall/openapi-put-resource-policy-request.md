---
description: PutResourcePolicyRequest schema from Amazon Network Firewall
layout: schema
name: PutResourcePolicyRequest
properties_list:
- description: ''
  name: ResourceArn
  type: object
- description: ''
  name: Policy
  type: object
provider_name: Amazon Network Firewall
provider_slug: amazon-network-firewall
schema_file: json-schema/openapi-put-resource-policy-request-schema.json
slug: openapi-put-resource-policy-request
source_filename: openapi-put-resource-policy-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-network-firewall/refs/heads/main/json-schema/openapi-put-resource-policy-request-schema.json\",\n  \"title\": \"PutResourcePolicyRequest\",\n  \"description\": \"PutResourcePolicyRequest schema from Amazon Network Firewall\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ResourceArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceArn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the account that you want to share rule groups and firewall policies with.\"\n        }\n      ]\n    },\n    \"Policy\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PolicyString\"\n        },\n        {\n          \"description\": \"<p>The IAM policy statement that lists the accounts that you want to share your rule group or firewall policy with\
  \ and the operations that you want the accounts to be able to perform. </p> <p>For a rule group resource, you can specify the following operations in the Actions section of the statement:</p> <ul> <li> <p>network-firewall:CreateFirewallPolicy</p> </li> <li> <p>network-firewall:UpdateFirewallPolicy</p> </li> <li> <p>network-firewall:ListRuleGroups</p> </li> </ul> <p>For a firewall policy resource, you can specify the following operations in the Actions section of the statement:</p> <ul> <li> <p>network-firewall:CreateFirewall</p> </li> <li> <p>network-firewall:UpdateFirewall</p> </li> <li> <p>network-firewall:AssociateFirewallPolicy</p> </li> <li> <p>network-firewall:ListFirewallPolicies</p> </li> </ul> <p>In the Resource section of the statement, you specify the ARNs for the rule groups and firewall policies that you want to share with the account that you specified in <code>Arn</code>.</p>\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"ResourceArn\",\n    \"Policy\"\n  ]\n\
  }"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-network-firewall/refs/heads/main/json-schema/openapi-put-resource-policy-request-schema.json
tags:
- AWS
- Firewall
- Intrusion Detection
- Network Security
- VPC
title: PutResourcePolicyRequest
---
