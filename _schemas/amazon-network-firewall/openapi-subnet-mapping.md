---
description: The ID for a subnet that you want to associate with the firewall. This is used with <a>CreateFirewall</a> and <a>AssociateSubnets</a>. Network Firewall creates an instance of the associated firewall in each subnet that you specify, to filter traffic in the subnet's Availability Zone.
layout: schema
name: SubnetMapping
properties_list:
- description: ''
  name: SubnetId
  type: object
- description: ''
  name: IPAddressType
  type: object
provider_name: Amazon Network Firewall
provider_slug: amazon-network-firewall
schema_file: json-schema/openapi-subnet-mapping-schema.json
slug: openapi-subnet-mapping
source_filename: openapi-subnet-mapping-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-network-firewall/refs/heads/main/json-schema/openapi-subnet-mapping-schema.json\",\n  \"title\": \"SubnetMapping\",\n  \"description\": \"The ID for a subnet that you want to associate with the firewall. This is used with <a>CreateFirewall</a> and <a>AssociateSubnets</a>. Network Firewall creates an instance of the associated firewall in each subnet that you specify, to filter traffic in the subnet's Availability Zone.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"SubnetId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CollectionMember_String\"\n        },\n        {\n          \"description\": \"The unique identifier for the subnet. \"\n        }\n      ]\n    },\n    \"IPAddressType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IPAddressType\"\n        },\n   \
  \     {\n          \"description\": \"The subnet's IP address type. You can't change the IP address type after you create the subnet.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"SubnetId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-network-firewall/refs/heads/main/json-schema/openapi-subnet-mapping-schema.json
tags:
- Firewall
- Intrusion Detection
- Network Security
- VPC
title: SubnetMapping
---
