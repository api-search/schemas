---
description: Describes a route table
layout: schema
name: RouteTable
properties_list:
- description: The ID of the route table
  name: routeTableId
  type: string
- description: The ID of the VPC
  name: vpcId
  type: string
- description: The routes in the route table
  name: routes
  type: array
- description: The associations between the route table and subnets or gateways
  name: associations
  type: array
- description: The ID of the AWS account that owns the route table
  name: ownerId
  type: string
- description: Any tags assigned to the route table
  name: tags
  type: array
provider_name: Amazon VPC
provider_slug: amazon-vpc
schema_file: json-schema/amazon-vpc-route-table-schema.json
slug: amazon-vpc-route-table
source_filename: amazon-vpc-route-table-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"description\": \"Describes a route table\",\n  \"properties\": {\n    \"routeTableId\": {\n      \"type\": \"string\",\n      \"description\": \"The ID of the route table\"\n    },\n    \"vpcId\": {\n      \"type\": \"string\",\n      \"description\": \"The ID of the VPC\"\n    },\n    \"routes\": {\n      \"type\": \"array\",\n      \"description\": \"The routes in the route table\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"destinationCidrBlock\": {\n            \"type\": \"string\",\n            \"description\": \"The IPv4 CIDR block used for the destination match\"\n          },\n          \"destinationIpv6CidrBlock\": {\n            \"type\": \"string\",\n            \"description\": \"The IPv6 CIDR block used for the destination match\"\n          },\n          \"gatewayId\": {\n            \"type\": \"string\",\n            \"description\": \"The ID of the gateway attached to your VPC\"\n\
  \          },\n          \"natGatewayId\": {\n            \"type\": \"string\",\n            \"description\": \"The ID of a NAT gateway\"\n          },\n          \"networkInterfaceId\": {\n            \"type\": \"string\",\n            \"description\": \"The ID of the network interface\"\n          },\n          \"state\": {\n            \"type\": \"string\",\n            \"description\": \"The state of the route\",\n            \"enum\": [\n              \"active\",\n              \"blackhole\"\n            ]\n          },\n          \"origin\": {\n            \"type\": \"string\",\n            \"description\": \"Describes how the route was created\",\n            \"enum\": [\n              \"CreateRouteTable\",\n              \"CreateRoute\",\n              \"EnableVgwRoutePropagation\"\n            ]\n          }\n        }\n      }\n    },\n    \"associations\": {\n      \"type\": \"array\",\n      \"description\": \"The associations between the route table and subnets or gateways\"\
  ,\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"routeTableAssociationId\": {\n            \"type\": \"string\"\n          },\n          \"routeTableId\": {\n            \"type\": \"string\"\n          },\n          \"subnetId\": {\n            \"type\": \"string\"\n          },\n          \"gatewayId\": {\n            \"type\": \"string\"\n          },\n          \"main\": {\n            \"type\": \"boolean\",\n            \"description\": \"Indicates whether this is the main route table\"\n          }\n        }\n      }\n    },\n    \"ownerId\": {\n      \"type\": \"string\",\n      \"description\": \"The ID of the AWS account that owns the route table\"\n    },\n    \"tags\": {\n      \"type\": \"array\",\n      \"description\": \"Any tags assigned to the route table\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/Tag\"\n      }\n    }\n  },\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"RouteTable\"\
  \n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-vpc/refs/heads/main/json-schema/amazon-vpc-route-table-schema.json
tags:
- Networking
- Private Cloud
- Security
- Subnets
- VPC
title: RouteTable
---
