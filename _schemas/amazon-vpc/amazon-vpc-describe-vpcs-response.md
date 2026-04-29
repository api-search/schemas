---
description: Response from the DescribeVpcs action
layout: schema
name: DescribeVpcsResponse
properties_list:
- description: Information about the VPCs
  name: vpcSet
  type: array
- description: Token for the next page of results
  name: nextToken
  type: string
provider_name: Amazon VPC
provider_slug: amazon-vpc
schema_file: json-schema/amazon-vpc-describe-vpcs-response-schema.json
slug: amazon-vpc-describe-vpcs-response
source_json: "{\n  \"type\": \"object\",\n  \"description\": \"Response from the DescribeVpcs action\",\n  \"properties\": {\n    \"vpcSet\": {\n      \"type\": \"array\",\n      \"description\": \"Information about the VPCs\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/Vpc\"\n      }\n    },\n    \"nextToken\": {\n      \"type\": \"string\",\n      \"description\": \"Token for the next page of results\"\n    }\n  },\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"DescribeVpcsResponse\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-vpc/refs/heads/main/json-schema/amazon-vpc-describe-vpcs-response-schema.json
tags:
- AWS
- Networking
- Private Cloud
- Security
- Subnets
- VPC
title: DescribeVpcsResponse
---
