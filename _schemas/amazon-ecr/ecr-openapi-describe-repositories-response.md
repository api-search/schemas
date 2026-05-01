---
description: DescribeRepositoriesResponse schema from Amazon ECR Amazon Elastic Container Registry (ECR) API
layout: schema
name: DescribeRepositoriesResponse
properties_list:
- description: ''
  name: repositories
  type: array
- description: ''
  name: nextToken
  type: string
provider_name: Amazon ECR
provider_slug: amazon-ecr
schema_file: json-schema/ecr-openapi-describe-repositories-response-schema.json
slug: ecr-openapi-describe-repositories-response
source_filename: ecr-openapi-describe-repositories-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-ecr/refs/heads/main/json-schema/ecr-openapi-describe-repositories-response-schema.json\",\n  \"title\": \"DescribeRepositoriesResponse\",\n  \"description\": \"DescribeRepositoriesResponse schema from Amazon ECR Amazon Elastic Container Registry (ECR) API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"repositories\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/Repository\"\n      }\n    },\n    \"nextToken\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ecr/refs/heads/main/json-schema/ecr-openapi-describe-repositories-response-schema.json
tags:
- Amazon Web Services
- Container Images
- Container Registry
- Containers
- Docker
- ECR
- OCI
title: DescribeRepositoriesResponse
---
