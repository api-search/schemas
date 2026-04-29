---
description: DescribeVpcEndpointServicesResult schema from Amazon PrivateLink API
layout: schema
name: DescribeVpcEndpointServicesResult
properties_list:
- description: List of supported service names
  name: ServiceNames
  type: array
- description: ''
  name: ServiceDetails
  type: array
- description: Token for next page of results
  name: NextToken
  type: string
provider_name: Amazon PrivateLink
provider_slug: amazon-privatelink
schema_file: json-schema/amazon-privatelink-describe-vpc-endpoint-services-result-schema.json
slug: amazon-privatelink-describe-vpc-endpoint-services-result
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-privatelink/refs/heads/main/json-schema/amazon-privatelink-describe-vpc-endpoint-services-result-schema.json\",\n  \"title\": \"DescribeVpcEndpointServicesResult\",\n  \"description\": \"DescribeVpcEndpointServicesResult schema from Amazon PrivateLink API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ServiceNames\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"List of supported service names\"\n    },\n    \"ServiceDetails\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/ServiceDetail\"\n      }\n    },\n    \"NextToken\": {\n      \"type\": \"string\",\n      \"description\": \"Token for next page of results\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-privatelink/refs/heads/main/json-schema/amazon-privatelink-describe-vpc-endpoint-services-result-schema.json
tags:
- AWS
- Networking
- Private Connectivity
- Security
- VPC
- Zero Trust
- Endpoint Services
title: DescribeVpcEndpointServicesResult
---
