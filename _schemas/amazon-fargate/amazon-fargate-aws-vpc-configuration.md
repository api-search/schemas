---
description: VPC configuration for awsvpc network mode
layout: schema
name: AwsVpcConfiguration
properties_list:
- description: Subnets for the task
  name: subnets
  type: array
- description: Security groups
  name: securityGroups
  type: array
- description: Whether to assign a public IP
  name: assignPublicIp
  type: string
provider_name: Amazon Fargate
provider_slug: amazon-fargate
schema_file: json-schema/amazon-fargate-aws-vpc-configuration-schema.json
slug: amazon-fargate-aws-vpc-configuration
source_filename: amazon-fargate-aws-vpc-configuration-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-fargate/refs/heads/main/json-schema/amazon-fargate-aws-vpc-configuration-schema.json\",\n  \"title\": \"AwsVpcConfiguration\",\n  \"description\": \"VPC configuration for awsvpc network mode\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"subnets\": {\n      \"type\": \"array\",\n      \"description\": \"Subnets for the task\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"example\": [\n        \"subnet-12345678\"\n      ]\n    },\n    \"securityGroups\": {\n      \"type\": \"array\",\n      \"description\": \"Security groups\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"example\": [\n        \"sg-12345678\"\n      ]\n    },\n    \"assignPublicIp\": {\n      \"type\": \"string\",\n      \"description\": \"Whether to assign a public IP\",\n      \"example\": \"ENABLED\",\n      \"enum\"\
  : [\n        \"ENABLED\",\n        \"DISABLED\"\n      ]\n    }\n  },\n  \"required\": [\n    \"subnets\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-fargate/refs/heads/main/json-schema/amazon-fargate-aws-vpc-configuration-schema.json
tags:
- Compute
- Containers
- ECS
- EKS
- Microservices
- Serverless
title: AwsVpcConfiguration
---
