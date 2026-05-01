---
description: Describes a NAT gateway
layout: schema
name: NatGateway
properties_list:
- description: The ID of the NAT gateway
  name: natGatewayId
  type: string
- description: The ID of the subnet in which the NAT gateway is located
  name: subnetId
  type: string
- description: The ID of the VPC in which the NAT gateway is located
  name: vpcId
  type: string
- description: The state of the NAT gateway
  name: state
  type: string
- description: Indicates whether the NAT gateway supports public or private connectivity
  name: connectivityType
  type: string
- description: Information about the IP addresses and network interface associated with the NAT gateway
  name: natGatewayAddresses
  type: array
- description: The date and time the NAT gateway was created
  name: createTime
  type: string
- description: Any tags assigned to the NAT gateway
  name: tags
  type: array
provider_name: Amazon VPC
provider_slug: amazon-vpc
schema_file: json-schema/amazon-vpc-nat-gateway-schema.json
slug: amazon-vpc-nat-gateway
source_filename: amazon-vpc-nat-gateway-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"description\": \"Describes a NAT gateway\",\n  \"properties\": {\n    \"natGatewayId\": {\n      \"type\": \"string\",\n      \"description\": \"The ID of the NAT gateway\"\n    },\n    \"subnetId\": {\n      \"type\": \"string\",\n      \"description\": \"The ID of the subnet in which the NAT gateway is located\"\n    },\n    \"vpcId\": {\n      \"type\": \"string\",\n      \"description\": \"The ID of the VPC in which the NAT gateway is located\"\n    },\n    \"state\": {\n      \"type\": \"string\",\n      \"description\": \"The state of the NAT gateway\",\n      \"enum\": [\n        \"pending\",\n        \"failed\",\n        \"available\",\n        \"deleting\",\n        \"deleted\"\n      ]\n    },\n    \"connectivityType\": {\n      \"type\": \"string\",\n      \"description\": \"Indicates whether the NAT gateway supports public or private connectivity\",\n      \"enum\": [\n        \"public\",\n        \"private\"\n      ]\n    },\n  \
  \  \"natGatewayAddresses\": {\n      \"type\": \"array\",\n      \"description\": \"Information about the IP addresses and network interface associated with the NAT gateway\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"allocationId\": {\n            \"type\": \"string\"\n          },\n          \"networkInterfaceId\": {\n            \"type\": \"string\"\n          },\n          \"privateIp\": {\n            \"type\": \"string\"\n          },\n          \"publicIp\": {\n            \"type\": \"string\"\n          }\n        }\n      }\n    },\n    \"createTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The date and time the NAT gateway was created\"\n    },\n    \"tags\": {\n      \"type\": \"array\",\n      \"description\": \"Any tags assigned to the NAT gateway\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/Tag\"\n      }\n    }\n  },\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\"\
  ,\n  \"title\": \"NatGateway\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-vpc/refs/heads/main/json-schema/amazon-vpc-nat-gateway-schema.json
tags:
- Networking
- Private Cloud
- Security
- Subnets
- VPC
title: NatGateway
---
