---
description: AssociateFirewallPolicyRequest schema from Amazon Network Firewall
layout: schema
name: AssociateFirewallPolicyRequest
properties_list:
- description: ''
  name: UpdateToken
  type: object
- description: ''
  name: FirewallArn
  type: object
- description: ''
  name: FirewallName
  type: object
- description: ''
  name: FirewallPolicyArn
  type: object
provider_name: Amazon Network Firewall
provider_slug: amazon-network-firewall
schema_file: json-schema/openapi-associate-firewall-policy-request-schema.json
slug: openapi-associate-firewall-policy-request
source_filename: openapi-associate-firewall-policy-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-network-firewall/refs/heads/main/json-schema/openapi-associate-firewall-policy-request-schema.json\",\n  \"title\": \"AssociateFirewallPolicyRequest\",\n  \"description\": \"AssociateFirewallPolicyRequest schema from Amazon Network Firewall\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"UpdateToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UpdateToken\"\n        },\n        {\n          \"description\": \"<p>An optional token that you can use for optimistic locking. Network Firewall returns a token to your requests that access the firewall. The token marks the state of the firewall resource at the time of the request. </p> <p>To make an unconditional change to the firewall, omit the token in your update request. Without the token, Network Firewall performs your updates regardless of whether the\
  \ firewall has changed since you last retrieved it.</p> <p>To make a conditional change to the firewall, provide the token in your update request. Network Firewall uses the token to ensure that the firewall hasn't changed since you last retrieved it. If it has changed, the operation fails with an <code>InvalidTokenException</code>. If this happens, retrieve the firewall again to get a current copy of it with a new token. Reapply your changes as needed, then try the operation again using the new token. </p>\"\n        }\n      ]\n    },\n    \"FirewallArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceArn\"\n        },\n        {\n          \"description\": \"<p>The Amazon Resource Name (ARN) of the firewall.</p> <p>You must specify the ARN or the name, and you can specify both. </p>\"\n        }\n      ]\n    },\n    \"FirewallName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceName\"\n        },\n      \
  \  {\n          \"description\": \"<p>The descriptive name of the firewall. You can't change the name of a firewall after you create it.</p> <p>You must specify the ARN or the name, and you can specify both. </p>\"\n        }\n      ]\n    },\n    \"FirewallPolicyArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceArn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the firewall policy.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"FirewallPolicyArn\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-network-firewall/refs/heads/main/json-schema/openapi-associate-firewall-policy-request-schema.json
tags:
- AWS
- Firewall
- Intrusion Detection
- Network Security
- VPC
title: AssociateFirewallPolicyRequest
---
