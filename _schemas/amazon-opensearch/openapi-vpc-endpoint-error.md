---
description: Error information when attempting to describe an Amazon OpenSearch Service-managed VPC endpoint.
layout: schema
name: VpcEndpointError
properties_list:
- description: ''
  name: VpcEndpointId
  type: object
- description: ''
  name: ErrorCode
  type: object
- description: ''
  name: ErrorMessage
  type: object
provider_name: Amazon OpenSearch Service API
provider_slug: amazon-opensearch
schema_file: json-schema/openapi-vpc-endpoint-error-schema.json
slug: openapi-vpc-endpoint-error
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-opensearch/refs/heads/main/json-schema/openapi-vpc-endpoint-error-schema.json\",\n  \"title\": \"VpcEndpointError\",\n  \"description\": \"Error information when attempting to describe an Amazon OpenSearch Service-managed VPC endpoint.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"VpcEndpointId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/VpcEndpointId\"\n        },\n        {\n          \"description\": \"The unique identifier of the endpoint. \"\n        }\n      ]\n    },\n    \"ErrorCode\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/VpcEndpointErrorCode\"\n        },\n        {\n          \"description\": \"The code associated with the error.\"\n        }\n      ]\n    },\n    \"ErrorMessage\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\
  \n        },\n        {\n          \"description\": \"A message describing the error.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-opensearch/refs/heads/main/json-schema/openapi-vpc-endpoint-error-schema.json
tags:
- Analytics
- AWS
- Elasticsearch
- Search
title: VpcEndpointError
---
