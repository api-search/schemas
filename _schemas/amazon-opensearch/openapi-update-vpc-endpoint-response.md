---
description: Contains the configuration and status of the VPC endpoint being updated.
layout: schema
name: UpdateVpcEndpointResponse
properties_list:
- description: ''
  name: VpcEndpoint
  type: object
provider_name: Amazon OpenSearch Service API
provider_slug: amazon-opensearch
schema_file: json-schema/openapi-update-vpc-endpoint-response-schema.json
slug: openapi-update-vpc-endpoint-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-opensearch/refs/heads/main/json-schema/openapi-update-vpc-endpoint-response-schema.json\",\n  \"title\": \"UpdateVpcEndpointResponse\",\n  \"description\": \"Contains the configuration and status of the VPC endpoint being updated.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"VpcEndpoint\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/VpcEndpoint\"\n        },\n        {\n          \"description\": \"The endpoint to be updated.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"VpcEndpoint\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-opensearch/refs/heads/main/json-schema/openapi-update-vpc-endpoint-response-schema.json
tags:
- Analytics
- AWS
- Elasticsearch
- Search
title: UpdateVpcEndpointResponse
---
