---
description: Summary information for an Amazon OpenSearch Service-managed VPC endpoint.
layout: schema
name: VpcEndpointSummary
properties_list:
- description: ''
  name: VpcEndpointId
  type: object
- description: ''
  name: VpcEndpointOwner
  type: object
- description: ''
  name: DomainArn
  type: object
- description: ''
  name: Status
  type: object
provider_name: Amazon OpenSearch Service API
provider_slug: amazon-opensearch
schema_file: json-schema/openapi-vpc-endpoint-summary-schema.json
slug: openapi-vpc-endpoint-summary
source_filename: openapi-vpc-endpoint-summary-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-opensearch/refs/heads/main/json-schema/openapi-vpc-endpoint-summary-schema.json\",\n  \"title\": \"VpcEndpointSummary\",\n  \"description\": \"Summary information for an Amazon OpenSearch Service-managed VPC endpoint.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"VpcEndpointId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/VpcEndpointId\"\n        },\n        {\n          \"description\": \"The unique identifier of the endpoint.\"\n        }\n      ]\n    },\n    \"VpcEndpointOwner\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The creator of the endpoint.\"\n        }\n      ]\n    },\n    \"DomainArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DomainArn\"\n        },\n\
  \        {\n          \"description\": \"The Amazon Resource Name (ARN) of the domain associated with the endpoint.\"\n        }\n      ]\n    },\n    \"Status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/VpcEndpointStatus\"\n        },\n        {\n          \"description\": \"The current status of the endpoint.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-opensearch/refs/heads/main/json-schema/openapi-vpc-endpoint-summary-schema.json
tags:
- Analytics
- Elasticsearch
- Search
title: VpcEndpointSummary
---
