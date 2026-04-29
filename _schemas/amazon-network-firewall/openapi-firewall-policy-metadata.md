---
description: High-level information about a firewall policy, returned by operations like create and describe. You can use the information provided in the metadata to retrieve and manage a firewall policy. You can retrieve all objects for a firewall policy by calling <a>DescribeFirewallPolicy</a>.
layout: schema
name: FirewallPolicyMetadata
properties_list:
- description: ''
  name: Name
  type: object
- description: ''
  name: Arn
  type: object
provider_name: Amazon Network Firewall
provider_slug: amazon-network-firewall
schema_file: json-schema/openapi-firewall-policy-metadata-schema.json
slug: openapi-firewall-policy-metadata
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-network-firewall/refs/heads/main/json-schema/openapi-firewall-policy-metadata-schema.json\",\n  \"title\": \"FirewallPolicyMetadata\",\n  \"description\": \"High-level information about a firewall policy, returned by operations like create and describe. You can use the information provided in the metadata to retrieve and manage a firewall policy. You can retrieve all objects for a firewall policy by calling <a>DescribeFirewallPolicy</a>. \",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceName\"\n        },\n        {\n          \"description\": \"The descriptive name of the firewall policy. You can't change the name of a firewall policy after you create it.\"\n        }\n      ]\n    },\n    \"Arn\": {\n      \"allOf\": [\n        {\n      \
  \    \"$ref\": \"#/components/schemas/ResourceArn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the firewall policy.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-network-firewall/refs/heads/main/json-schema/openapi-firewall-policy-metadata-schema.json
tags:
- AWS
- Firewall
- Intrusion Detection
- Network Security
- VPC
title: FirewallPolicyMetadata
---
