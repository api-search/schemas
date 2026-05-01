---
description: Network configuration for the task
layout: schema
name: NetworkConfiguration
properties_list:
- description: ''
  name: awsvpcConfiguration
  type: object
provider_name: Amazon Fargate
provider_slug: amazon-fargate
schema_file: json-schema/amazon-fargate-network-configuration-schema.json
slug: amazon-fargate-network-configuration
source_filename: amazon-fargate-network-configuration-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-fargate/refs/heads/main/json-schema/amazon-fargate-network-configuration-schema.json\",\n  \"title\": \"NetworkConfiguration\",\n  \"description\": \"Network configuration for the task\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"awsvpcConfiguration\": {\n      \"$ref\": \"#/components/schemas/AwsVpcConfiguration\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-fargate/refs/heads/main/json-schema/amazon-fargate-network-configuration-schema.json
tags:
- Compute
- Containers
- ECS
- EKS
- Microservices
- Serverless
title: NetworkConfiguration
---
