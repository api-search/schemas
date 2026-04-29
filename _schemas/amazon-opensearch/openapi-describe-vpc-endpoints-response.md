---
description: Container for response parameters to the <code><a>DescribeVpcEndpoints</a></code> operation. Returns a list containing configuration details and status of the VPC Endpoints as well as a list containing error responses of the endpoints that could not be described
layout: schema
name: DescribeVpcEndpointsResponse
properties_list:
- description: ''
  name: VpcEndpoints
  type: object
- description: ''
  name: VpcEndpointErrors
  type: object
provider_name: Amazon OpenSearch Service API
provider_slug: amazon-opensearch
schema_file: json-schema/openapi-describe-vpc-endpoints-response-schema.json
slug: openapi-describe-vpc-endpoints-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-opensearch/refs/heads/main/json-schema/openapi-describe-vpc-endpoints-response-schema.json\",\n  \"title\": \"DescribeVpcEndpointsResponse\",\n  \"description\": \"Container for response parameters to the <code><a>DescribeVpcEndpoints</a></code> operation. Returns a list containing configuration details and status of the VPC Endpoints as well as a list containing error responses of the endpoints that could not be described\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"VpcEndpoints\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/VpcEndpoints\"\n        },\n        {\n          \"description\": \"Information about each requested VPC endpoint.\"\n        }\n      ]\n    },\n    \"VpcEndpointErrors\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/VpcEndpointErrorList\"\n\
  \        },\n        {\n          \"description\": \"Any errors associated with the request.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"VpcEndpoints\",\n    \"VpcEndpointErrors\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-opensearch/refs/heads/main/json-schema/openapi-describe-vpc-endpoints-response-schema.json
tags:
- Analytics
- AWS
- Elasticsearch
- Search
title: DescribeVpcEndpointsResponse
---
