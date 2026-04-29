---
description: Container for the parameters to the <code><a>CreateVpcEndpointRequest</a></code> operation.
layout: schema
name: CreateVpcEndpointRequest
properties_list:
- description: ''
  name: DomainArn
  type: object
- description: ''
  name: VpcOptions
  type: object
- description: ''
  name: ClientToken
  type: object
provider_name: Amazon OpenSearch Service API
provider_slug: amazon-opensearch
schema_file: json-schema/openapi-create-vpc-endpoint-request-schema.json
slug: openapi-create-vpc-endpoint-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-opensearch/refs/heads/main/json-schema/openapi-create-vpc-endpoint-request-schema.json\",\n  \"title\": \"CreateVpcEndpointRequest\",\n  \"description\": \"Container for the parameters to the <code><a>CreateVpcEndpointRequest</a></code> operation.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"DomainArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DomainArn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the domain to grant access to.\"\n        }\n      ]\n    },\n    \"VpcOptions\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/VPCOptions\"\n        },\n        {\n          \"description\": \"Options to specify the subnets and security groups for the endpoint.\"\n        }\n      ]\n    },\n    \"ClientToken\": {\n      \"\
  allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ClientToken\"\n        },\n        {\n          \"description\": \"Unique, case-sensitive identifier to ensure idempotency of the request.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"DomainArn\",\n    \"VpcOptions\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-opensearch/refs/heads/main/json-schema/openapi-create-vpc-endpoint-request-schema.json
tags:
- Analytics
- AWS
- Elasticsearch
- Search
title: CreateVpcEndpointRequest
---
