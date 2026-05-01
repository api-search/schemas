---
description: Response from the DescribeSubnets action
layout: schema
name: DescribeSubnetsResponse
properties_list:
- description: Information about the subnets
  name: subnetSet
  type: array
- description: Token for the next page of results
  name: nextToken
  type: string
provider_name: Amazon VPC
provider_slug: amazon-vpc
schema_file: json-schema/amazon-vpc-describe-subnets-response-schema.json
slug: amazon-vpc-describe-subnets-response
source_filename: amazon-vpc-describe-subnets-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"description\": \"Response from the DescribeSubnets action\",\n  \"properties\": {\n    \"subnetSet\": {\n      \"type\": \"array\",\n      \"description\": \"Information about the subnets\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/Subnet\"\n      }\n    },\n    \"nextToken\": {\n      \"type\": \"string\",\n      \"description\": \"Token for the next page of results\"\n    }\n  },\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"DescribeSubnetsResponse\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-vpc/refs/heads/main/json-schema/amazon-vpc-describe-subnets-response-schema.json
tags:
- Networking
- Private Cloud
- Security
- Subnets
- VPC
title: DescribeSubnetsResponse
---
