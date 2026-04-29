---
description: Describes an internet gateway
layout: schema
name: InternetGateway
properties_list:
- description: The ID of the internet gateway
  name: internetGatewayId
  type: string
- description: Any VPCs attached to the internet gateway
  name: attachments
  type: array
- description: The ID of the AWS account that owns the internet gateway
  name: ownerId
  type: string
- description: Any tags assigned to the internet gateway
  name: tags
  type: array
provider_name: Amazon VPC
provider_slug: amazon-vpc
schema_file: json-schema/amazon-vpc-internet-gateway-schema.json
slug: amazon-vpc-internet-gateway
source_json: "{\n  \"type\": \"object\",\n  \"description\": \"Describes an internet gateway\",\n  \"properties\": {\n    \"internetGatewayId\": {\n      \"type\": \"string\",\n      \"description\": \"The ID of the internet gateway\"\n    },\n    \"attachments\": {\n      \"type\": \"array\",\n      \"description\": \"Any VPCs attached to the internet gateway\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"state\": {\n            \"type\": \"string\",\n            \"description\": \"The current state of the attachment\",\n            \"enum\": [\n              \"attaching\",\n              \"attached\",\n              \"detaching\",\n              \"detached\"\n            ]\n          },\n          \"vpcId\": {\n            \"type\": \"string\",\n            \"description\": \"The ID of the VPC\"\n          }\n        }\n      }\n    },\n    \"ownerId\": {\n      \"type\": \"string\",\n      \"description\": \"The ID of the AWS account that\
  \ owns the internet gateway\"\n    },\n    \"tags\": {\n      \"type\": \"array\",\n      \"description\": \"Any tags assigned to the internet gateway\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/Tag\"\n      }\n    }\n  },\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"InternetGateway\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-vpc/refs/heads/main/json-schema/amazon-vpc-internet-gateway-schema.json
tags:
- AWS
- Networking
- Private Cloud
- Security
- Subnets
- VPC
title: InternetGateway
---
