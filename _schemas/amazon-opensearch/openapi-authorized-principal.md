---
description: Information about an account or service that has access to an Amazon OpenSearch Service domain through the use of an interface VPC endpoint.
layout: schema
name: AuthorizedPrincipal
properties_list:
- description: ''
  name: PrincipalType
  type: object
- description: ''
  name: Principal
  type: object
provider_name: Amazon OpenSearch Service API
provider_slug: amazon-opensearch
schema_file: json-schema/openapi-authorized-principal-schema.json
slug: openapi-authorized-principal
source_filename: openapi-authorized-principal-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-opensearch/refs/heads/main/json-schema/openapi-authorized-principal-schema.json\",\n  \"title\": \"AuthorizedPrincipal\",\n  \"description\": \"Information about an account or service that has access to an Amazon OpenSearch Service domain through the use of an interface VPC endpoint.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"PrincipalType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PrincipalType\"\n        },\n        {\n          \"description\": \"The type of principal.\"\n        }\n      ]\n    },\n    \"Principal\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The IAM principal that is allowed access to the domain.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-opensearch/refs/heads/main/json-schema/openapi-authorized-principal-schema.json
tags:
- Analytics
- AWS
- Elasticsearch
- Search
title: AuthorizedPrincipal
---
