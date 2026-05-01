---
description: Container for request parameters to the <code><a>DescribeVpcEndpoints</a></code> operation. Specifies the list of VPC endpoints to be described.
layout: schema
name: DescribeVpcEndpointsRequest
properties_list:
- description: ''
  name: VpcEndpointIds
  type: object
provider_name: Amazon OpenSearch Service API
provider_slug: amazon-opensearch
schema_file: json-schema/openapi-describe-vpc-endpoints-request-schema.json
slug: openapi-describe-vpc-endpoints-request
source_filename: openapi-describe-vpc-endpoints-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-opensearch/refs/heads/main/json-schema/openapi-describe-vpc-endpoints-request-schema.json\",\n  \"title\": \"DescribeVpcEndpointsRequest\",\n  \"description\": \"Container for request parameters to the <code><a>DescribeVpcEndpoints</a></code> operation. Specifies the list of VPC endpoints to be described.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"VpcEndpointIds\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/VpcEndpointIdList\"\n        },\n        {\n          \"description\": \"The unique identifiers of the endpoints to get information about.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"VpcEndpointIds\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-opensearch/refs/heads/main/json-schema/openapi-describe-vpc-endpoints-request-schema.json
tags:
- Analytics
- Elasticsearch
- Search
title: DescribeVpcEndpointsRequest
---
