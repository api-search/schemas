---
description: DescribeFirewallPolicyRequest schema from Amazon Network Firewall
layout: schema
name: DescribeFirewallPolicyRequest
properties_list:
- description: ''
  name: FirewallPolicyName
  type: object
- description: ''
  name: FirewallPolicyArn
  type: object
provider_name: Amazon Network Firewall
provider_slug: amazon-network-firewall
schema_file: json-schema/openapi-describe-firewall-policy-request-schema.json
slug: openapi-describe-firewall-policy-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-network-firewall/refs/heads/main/json-schema/openapi-describe-firewall-policy-request-schema.json\",\n  \"title\": \"DescribeFirewallPolicyRequest\",\n  \"description\": \"DescribeFirewallPolicyRequest schema from Amazon Network Firewall\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"FirewallPolicyName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceName\"\n        },\n        {\n          \"description\": \"<p>The descriptive name of the firewall policy. You can't change the name of a firewall policy after you create it.</p> <p>You must specify the ARN or the name, and you can specify both. </p>\"\n        }\n      ]\n    },\n    \"FirewallPolicyArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceArn\"\n        },\n        {\n          \"description\"\
  : \"<p>The Amazon Resource Name (ARN) of the firewall policy.</p> <p>You must specify the ARN or the name, and you can specify both. </p>\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-network-firewall/refs/heads/main/json-schema/openapi-describe-firewall-policy-request-schema.json
tags:
- AWS
- Firewall
- Intrusion Detection
- Network Security
- VPC
title: DescribeFirewallPolicyRequest
---
