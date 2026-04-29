---
description: DescribeVpcEndpointsResult schema from Amazon PrivateLink API
layout: schema
name: DescribeVpcEndpointsResult
properties_list:
- description: ''
  name: VpcEndpoints
  type: array
- description: ''
  name: NextToken
  type: string
provider_name: Amazon PrivateLink
provider_slug: amazon-privatelink
schema_file: json-schema/amazon-privatelink-describe-vpc-endpoints-result-schema.json
slug: amazon-privatelink-describe-vpc-endpoints-result
source_filename: amazon-privatelink-describe-vpc-endpoints-result-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-privatelink/refs/heads/main/json-schema/amazon-privatelink-describe-vpc-endpoints-result-schema.json\",\n  \"title\": \"DescribeVpcEndpointsResult\",\n  \"description\": \"DescribeVpcEndpointsResult schema from Amazon PrivateLink API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"VpcEndpoints\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/VpcEndpoint\"\n      }\n    },\n    \"NextToken\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-privatelink/refs/heads/main/json-schema/amazon-privatelink-describe-vpc-endpoints-result-schema.json
tags:
- AWS
- Networking
- Private Connectivity
- Security
- VPC
- Zero Trust
- Endpoint Services
title: DescribeVpcEndpointsResult
---
