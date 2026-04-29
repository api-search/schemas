---
description: DescribeFirewallResponse schema from Amazon Network Firewall
layout: schema
name: DescribeFirewallResponse
properties_list:
- description: ''
  name: UpdateToken
  type: object
- description: ''
  name: Firewall
  type: object
- description: ''
  name: FirewallStatus
  type: object
provider_name: Amazon Network Firewall
provider_slug: amazon-network-firewall
schema_file: json-schema/openapi-describe-firewall-response-schema.json
slug: openapi-describe-firewall-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-network-firewall/refs/heads/main/json-schema/openapi-describe-firewall-response-schema.json\",\n  \"title\": \"DescribeFirewallResponse\",\n  \"description\": \"DescribeFirewallResponse schema from Amazon Network Firewall\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"UpdateToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UpdateToken\"\n        },\n        {\n          \"description\": \"<p>An optional token that you can use for optimistic locking. Network Firewall returns a token to your requests that access the firewall. The token marks the state of the firewall resource at the time of the request. </p> <p>To make an unconditional change to the firewall, omit the token in your update request. Without the token, Network Firewall performs your updates regardless of whether the firewall has changed\
  \ since you last retrieved it.</p> <p>To make a conditional change to the firewall, provide the token in your update request. Network Firewall uses the token to ensure that the firewall hasn't changed since you last retrieved it. If it has changed, the operation fails with an <code>InvalidTokenException</code>. If this happens, retrieve the firewall again to get a current copy of it with a new token. Reapply your changes as needed, then try the operation again using the new token. </p>\"\n        }\n      ]\n    },\n    \"Firewall\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Firewall\"\n        },\n        {\n          \"description\": \"The configuration settings for the firewall. These settings include the firewall policy and the subnets in your VPC to use for the firewall endpoints. \"\n        }\n      ]\n    },\n    \"FirewallStatus\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FirewallStatus\"\n        },\n    \
  \    {\n          \"description\": \"Detailed information about the current status of a <a>Firewall</a>. You can retrieve this for a firewall by calling <a>DescribeFirewall</a> and providing the firewall name and ARN.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-network-firewall/refs/heads/main/json-schema/openapi-describe-firewall-response-schema.json
tags:
- AWS
- Firewall
- Intrusion Detection
- Network Security
- VPC
title: DescribeFirewallResponse
---
