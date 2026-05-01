---
description: Modifies an Amazon OpenSearch Service-managed interface VPC endpoint.
layout: schema
name: UpdateVpcEndpointRequest
properties_list:
- description: ''
  name: VpcEndpointId
  type: object
- description: ''
  name: VpcOptions
  type: object
provider_name: Amazon OpenSearch Service API
provider_slug: amazon-opensearch
schema_file: json-schema/openapi-update-vpc-endpoint-request-schema.json
slug: openapi-update-vpc-endpoint-request
source_filename: openapi-update-vpc-endpoint-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-opensearch/refs/heads/main/json-schema/openapi-update-vpc-endpoint-request-schema.json\",\n  \"title\": \"UpdateVpcEndpointRequest\",\n  \"description\": \"Modifies an Amazon OpenSearch Service-managed interface VPC endpoint.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"VpcEndpointId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/VpcEndpointId\"\n        },\n        {\n          \"description\": \"Unique identifier of the VPC endpoint to be updated.\"\n        }\n      ]\n    },\n    \"VpcOptions\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/VPCOptions\"\n        },\n        {\n          \"description\": \"The security groups and/or subnets to add, remove, or modify.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"VpcEndpointId\",\n    \"VpcOptions\"\
  \n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-opensearch/refs/heads/main/json-schema/openapi-update-vpc-endpoint-request-schema.json
tags:
- Analytics
- Elasticsearch
- Search
title: UpdateVpcEndpointRequest
---
