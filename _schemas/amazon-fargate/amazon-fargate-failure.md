---
description: A failure returned by an API operation
layout: schema
name: Failure
properties_list:
- description: ARN of the resource that failed
  name: arn
  type: string
- description: Reason for the failure
  name: reason
  type: string
- description: Additional detail about the failure
  name: detail
  type: string
provider_name: Amazon Fargate
provider_slug: amazon-fargate
schema_file: json-schema/amazon-fargate-failure-schema.json
slug: amazon-fargate-failure
source_filename: amazon-fargate-failure-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-fargate/refs/heads/main/json-schema/amazon-fargate-failure-schema.json\",\n  \"title\": \"Failure\",\n  \"description\": \"A failure returned by an API operation\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"arn\": {\n      \"type\": \"string\",\n      \"description\": \"ARN of the resource that failed\",\n      \"example\": \"arn:aws:ecs:us-east-1:123456789012:cluster/missing-cluster\"\n    },\n    \"reason\": {\n      \"type\": \"string\",\n      \"description\": \"Reason for the failure\",\n      \"example\": \"MISSING\"\n    },\n    \"detail\": {\n      \"type\": \"string\",\n      \"description\": \"Additional detail about the failure\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-fargate/refs/heads/main/json-schema/amazon-fargate-failure-schema.json
tags:
- AWS
- Compute
- Containers
- ECS
- EKS
- Microservices
- Serverless
title: Failure
---
