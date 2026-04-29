---
description: DescribeVpcEndpointConnectionsResult schema from Amazon PrivateLink API
layout: schema
name: DescribeVpcEndpointConnectionsResult
properties_list:
- description: ''
  name: VpcEndpointConnections
  type: array
- description: ''
  name: NextToken
  type: string
provider_name: Amazon PrivateLink
provider_slug: amazon-privatelink
schema_file: json-schema/amazon-privatelink-describe-vpc-endpoint-connections-result-schema.json
slug: amazon-privatelink-describe-vpc-endpoint-connections-result
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-privatelink/refs/heads/main/json-schema/amazon-privatelink-describe-vpc-endpoint-connections-result-schema.json\",\n  \"title\": \"DescribeVpcEndpointConnectionsResult\",\n  \"description\": \"DescribeVpcEndpointConnectionsResult schema from Amazon PrivateLink API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"VpcEndpointConnections\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/VpcEndpointConnection\"\n      }\n    },\n    \"NextToken\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-privatelink/refs/heads/main/json-schema/amazon-privatelink-describe-vpc-endpoint-connections-result-schema.json
tags:
- AWS
- Networking
- Private Connectivity
- Security
- VPC
- Zero Trust
- Endpoint Services
title: DescribeVpcEndpointConnectionsResult
---
