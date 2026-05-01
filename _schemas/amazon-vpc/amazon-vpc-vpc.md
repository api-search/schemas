---
description: Describes a VPC
layout: schema
name: Vpc
properties_list:
- description: The ID of the VPC
  name: vpcId
  type: string
- description: The current state of the VPC
  name: state
  type: string
- description: The primary IPv4 CIDR block for the VPC
  name: cidrBlock
  type: string
- description: Information about the IPv4 CIDR blocks associated with the VPC
  name: cidrBlockAssociationSet
  type: array
- description: Information about the IPv6 CIDR blocks associated with the VPC
  name: ipv6CidrBlockAssociationSet
  type: array
- description: The ID of the set of DHCP options associated with the VPC
  name: dhcpOptionsId
  type: string
- description: The allowed tenancy of instances launched into the VPC
  name: instanceTenancy
  type: string
- description: Indicates whether the VPC is the default VPC
  name: isDefault
  type: boolean
- description: The ID of the AWS account that owns the VPC
  name: ownerId
  type: string
- description: Any tags assigned to the VPC
  name: tags
  type: array
provider_name: Amazon VPC
provider_slug: amazon-vpc
schema_file: json-schema/amazon-vpc-vpc-schema.json
slug: amazon-vpc-vpc
source_filename: amazon-vpc-vpc-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"description\": \"Describes a VPC\",\n  \"properties\": {\n    \"vpcId\": {\n      \"type\": \"string\",\n      \"description\": \"The ID of the VPC\"\n    },\n    \"state\": {\n      \"type\": \"string\",\n      \"description\": \"The current state of the VPC\",\n      \"enum\": [\n        \"pending\",\n        \"available\"\n      ]\n    },\n    \"cidrBlock\": {\n      \"type\": \"string\",\n      \"description\": \"The primary IPv4 CIDR block for the VPC\"\n    },\n    \"cidrBlockAssociationSet\": {\n      \"type\": \"array\",\n      \"description\": \"Information about the IPv4 CIDR blocks associated with the VPC\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"cidrBlock\": {\n            \"type\": \"string\"\n          },\n          \"associationId\": {\n            \"type\": \"string\"\n          },\n          \"cidrBlockState\": {\n            \"type\": \"object\",\n            \"properties\"\
  : {\n              \"state\": {\n                \"type\": \"string\"\n              }\n            }\n          }\n        }\n      }\n    },\n    \"ipv6CidrBlockAssociationSet\": {\n      \"type\": \"array\",\n      \"description\": \"Information about the IPv6 CIDR blocks associated with the VPC\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"ipv6CidrBlock\": {\n            \"type\": \"string\"\n          },\n          \"associationId\": {\n            \"type\": \"string\"\n          },\n          \"ipv6CidrBlockState\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"state\": {\n                \"type\": \"string\"\n              }\n            }\n          }\n        }\n      }\n    },\n    \"dhcpOptionsId\": {\n      \"type\": \"string\",\n      \"description\": \"The ID of the set of DHCP options associated with the VPC\"\n    },\n    \"instanceTenancy\": {\n      \"type\": \"string\",\n      \"description\"\
  : \"The allowed tenancy of instances launched into the VPC\",\n      \"enum\": [\n        \"default\",\n        \"dedicated\",\n        \"host\"\n      ]\n    },\n    \"isDefault\": {\n      \"type\": \"boolean\",\n      \"description\": \"Indicates whether the VPC is the default VPC\"\n    },\n    \"ownerId\": {\n      \"type\": \"string\",\n      \"description\": \"The ID of the AWS account that owns the VPC\"\n    },\n    \"tags\": {\n      \"type\": \"array\",\n      \"description\": \"Any tags assigned to the VPC\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/Tag\"\n      }\n    }\n  },\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"Vpc\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-vpc/refs/heads/main/json-schema/amazon-vpc-vpc-schema.json
tags:
- Networking
- Private Cloud
- Security
- Subnets
- VPC
title: Vpc
---
