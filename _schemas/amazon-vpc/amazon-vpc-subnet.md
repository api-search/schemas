---
description: Describes a subnet
layout: schema
name: Subnet
properties_list:
- description: The ID of the subnet
  name: subnetId
  type: string
- description: The Amazon Resource Name (ARN) of the subnet
  name: subnetArn
  type: string
- description: The ID of the VPC the subnet is in
  name: vpcId
  type: string
- description: The current state of the subnet
  name: state
  type: string
- description: The IPv4 CIDR block assigned to the subnet
  name: cidrBlock
  type: string
- description: The Availability Zone of the subnet
  name: availabilityZone
  type: string
- description: The AZ ID of the subnet
  name: availabilityZoneId
  type: string
- description: The number of unused private IPv4 addresses in the subnet
  name: availableIpAddressCount
  type: integer
- description: Indicates whether this is the default subnet for the Availability Zone
  name: defaultForAz
  type: boolean
- description: Indicates whether instances launched in this subnet receive a public IPv4 address
  name: mapPublicIpOnLaunch
  type: boolean
- description: The ID of the AWS account that owns the subnet
  name: ownerId
  type: string
- description: Any tags assigned to the subnet
  name: tags
  type: array
provider_name: Amazon VPC
provider_slug: amazon-vpc
schema_file: json-schema/amazon-vpc-subnet-schema.json
slug: amazon-vpc-subnet
source_json: "{\n  \"type\": \"object\",\n  \"description\": \"Describes a subnet\",\n  \"properties\": {\n    \"subnetId\": {\n      \"type\": \"string\",\n      \"description\": \"The ID of the subnet\"\n    },\n    \"subnetArn\": {\n      \"type\": \"string\",\n      \"description\": \"The Amazon Resource Name (ARN) of the subnet\"\n    },\n    \"vpcId\": {\n      \"type\": \"string\",\n      \"description\": \"The ID of the VPC the subnet is in\"\n    },\n    \"state\": {\n      \"type\": \"string\",\n      \"description\": \"The current state of the subnet\",\n      \"enum\": [\n        \"pending\",\n        \"available\"\n      ]\n    },\n    \"cidrBlock\": {\n      \"type\": \"string\",\n      \"description\": \"The IPv4 CIDR block assigned to the subnet\"\n    },\n    \"availabilityZone\": {\n      \"type\": \"string\",\n      \"description\": \"The Availability Zone of the subnet\"\n    },\n    \"availabilityZoneId\": {\n      \"type\": \"string\",\n      \"description\": \"The\
  \ AZ ID of the subnet\"\n    },\n    \"availableIpAddressCount\": {\n      \"type\": \"integer\",\n      \"description\": \"The number of unused private IPv4 addresses in the subnet\"\n    },\n    \"defaultForAz\": {\n      \"type\": \"boolean\",\n      \"description\": \"Indicates whether this is the default subnet for the Availability Zone\"\n    },\n    \"mapPublicIpOnLaunch\": {\n      \"type\": \"boolean\",\n      \"description\": \"Indicates whether instances launched in this subnet receive a public IPv4 address\"\n    },\n    \"ownerId\": {\n      \"type\": \"string\",\n      \"description\": \"The ID of the AWS account that owns the subnet\"\n    },\n    \"tags\": {\n      \"type\": \"array\",\n      \"description\": \"Any tags assigned to the subnet\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/Tag\"\n      }\n    }\n  },\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"Subnet\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-vpc/refs/heads/main/json-schema/amazon-vpc-subnet-schema.json
tags:
- AWS
- Networking
- Private Cloud
- Security
- Subnets
- VPC
title: Subnet
---
