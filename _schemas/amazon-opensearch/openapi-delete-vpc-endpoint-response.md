---
description: Container for response parameters to the <code><a>DeleteVpcEndpoint</a></code> operation. Contains the summarized detail of the VPC Endpoint being deleted.
layout: schema
name: DeleteVpcEndpointResponse
properties_list:
- description: ''
  name: VpcEndpointSummary
  type: object
provider_name: Amazon OpenSearch Service API
provider_slug: amazon-opensearch
schema_file: json-schema/openapi-delete-vpc-endpoint-response-schema.json
slug: openapi-delete-vpc-endpoint-response
source_filename: openapi-delete-vpc-endpoint-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-opensearch/refs/heads/main/json-schema/openapi-delete-vpc-endpoint-response-schema.json\",\n  \"title\": \"DeleteVpcEndpointResponse\",\n  \"description\": \"Container for response parameters to the <code><a>DeleteVpcEndpoint</a></code> operation. Contains the summarized detail of the VPC Endpoint being deleted.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"VpcEndpointSummary\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/VpcEndpointSummary\"\n        },\n        {\n          \"description\": \"Information about the deleted endpoint, including its current status (<code>DELETING</code> or <code>DELETE_FAILED</code>).\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"VpcEndpointSummary\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-opensearch/refs/heads/main/json-schema/openapi-delete-vpc-endpoint-response-schema.json
tags:
- Analytics
- Elasticsearch
- Search
title: DeleteVpcEndpointResponse
---
