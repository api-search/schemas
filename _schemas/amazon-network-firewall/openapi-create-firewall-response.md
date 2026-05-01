---
description: CreateFirewallResponse schema from Amazon Network Firewall
layout: schema
name: CreateFirewallResponse
properties_list:
- description: ''
  name: Firewall
  type: object
- description: ''
  name: FirewallStatus
  type: object
provider_name: Amazon Network Firewall
provider_slug: amazon-network-firewall
schema_file: json-schema/openapi-create-firewall-response-schema.json
slug: openapi-create-firewall-response
source_filename: openapi-create-firewall-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-network-firewall/refs/heads/main/json-schema/openapi-create-firewall-response-schema.json\",\n  \"title\": \"CreateFirewallResponse\",\n  \"description\": \"CreateFirewallResponse schema from Amazon Network Firewall\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Firewall\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Firewall\"\n        },\n        {\n          \"description\": \"The configuration settings for the firewall. These settings include the firewall policy and the subnets in your VPC to use for the firewall endpoints. \"\n        }\n      ]\n    },\n    \"FirewallStatus\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FirewallStatus\"\n        },\n        {\n          \"description\": \"Detailed information about the current status of a <a>Firewall</a>. You\
  \ can retrieve this for a firewall by calling <a>DescribeFirewall</a> and providing the firewall name and ARN.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-network-firewall/refs/heads/main/json-schema/openapi-create-firewall-response-schema.json
tags:
- Firewall
- Intrusion Detection
- Network Security
- VPC
title: CreateFirewallResponse
---
