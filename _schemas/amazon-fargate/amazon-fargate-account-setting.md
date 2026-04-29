---
description: An ECS account setting
layout: schema
name: AccountSetting
properties_list:
- description: Setting name
  name: name
  type: string
- description: Setting value
  name: value
  type: string
- description: Principal ARN
  name: principalArn
  type: string
provider_name: Amazon Fargate
provider_slug: amazon-fargate
schema_file: json-schema/amazon-fargate-account-setting-schema.json
slug: amazon-fargate-account-setting
source_filename: amazon-fargate-account-setting-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-fargate/refs/heads/main/json-schema/amazon-fargate-account-setting-schema.json\",\n  \"title\": \"AccountSetting\",\n  \"description\": \"An ECS account setting\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Setting name\",\n      \"example\": \"containerInsights\"\n    },\n    \"value\": {\n      \"type\": \"string\",\n      \"description\": \"Setting value\",\n      \"example\": \"enabled\"\n    },\n    \"principalArn\": {\n      \"type\": \"string\",\n      \"description\": \"Principal ARN\",\n      \"example\": \"arn:aws:iam::123456789012:root\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-fargate/refs/heads/main/json-schema/amazon-fargate-account-setting-schema.json
tags:
- AWS
- Compute
- Containers
- ECS
- EKS
- Microservices
- Serverless
title: AccountSetting
---
