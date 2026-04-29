---
description: Container for response parameters to the <code><a>CreateVpcEndpoint</a></code> operation. Contains the configuration and status of the VPC Endpoint being created.
layout: schema
name: CreateVpcEndpointResponse
properties_list:
- description: ''
  name: VpcEndpoint
  type: object
provider_name: Amazon OpenSearch Service API
provider_slug: amazon-opensearch
schema_file: json-schema/openapi-create-vpc-endpoint-response-schema.json
slug: openapi-create-vpc-endpoint-response
source_filename: openapi-create-vpc-endpoint-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-opensearch/refs/heads/main/json-schema/openapi-create-vpc-endpoint-response-schema.json\",\n  \"title\": \"CreateVpcEndpointResponse\",\n  \"description\": \"Container for response parameters to the <code><a>CreateVpcEndpoint</a></code> operation. Contains the configuration and status of the VPC Endpoint being created.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"VpcEndpoint\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/VpcEndpoint\"\n        },\n        {\n          \"description\": \"Information about the newly created VPC endpoint.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"VpcEndpoint\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-opensearch/refs/heads/main/json-schema/openapi-create-vpc-endpoint-response-schema.json
tags:
- Analytics
- AWS
- Elasticsearch
- Search
title: CreateVpcEndpointResponse
---
