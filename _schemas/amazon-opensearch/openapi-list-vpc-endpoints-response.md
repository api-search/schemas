---
description: Container for response parameters to the <code><a>ListVpcEndpoints</a></code> operation. Returns a list containing summarized details of the VPC endpoints.
layout: schema
name: ListVpcEndpointsResponse
properties_list:
- description: ''
  name: VpcEndpointSummaryList
  type: object
- description: ''
  name: NextToken
  type: object
provider_name: Amazon OpenSearch Service API
provider_slug: amazon-opensearch
schema_file: json-schema/openapi-list-vpc-endpoints-response-schema.json
slug: openapi-list-vpc-endpoints-response
source_filename: openapi-list-vpc-endpoints-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-opensearch/refs/heads/main/json-schema/openapi-list-vpc-endpoints-response-schema.json\",\n  \"title\": \"ListVpcEndpointsResponse\",\n  \"description\": \"Container for response parameters to the <code><a>ListVpcEndpoints</a></code> operation. Returns a list containing summarized details of the VPC endpoints.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"VpcEndpointSummaryList\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/VpcEndpointSummaryList\"\n        },\n        {\n          \"description\": \"Information about each endpoint.\"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NextToken\"\n        },\n        {\n          \"description\": \"Provides an identifier to allow retrieval of paginated results.\"\n        }\n\
  \      ]\n    }\n  },\n  \"required\": [\n    \"VpcEndpointSummaryList\",\n    \"NextToken\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-opensearch/refs/heads/main/json-schema/openapi-list-vpc-endpoints-response-schema.json
tags:
- Analytics
- AWS
- Elasticsearch
- Search
title: ListVpcEndpointsResponse
---
