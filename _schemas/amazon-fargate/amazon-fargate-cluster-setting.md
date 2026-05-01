---
description: A cluster setting
layout: schema
name: ClusterSetting
properties_list:
- description: Setting name
  name: name
  type: string
- description: Setting value
  name: value
  type: string
provider_name: Amazon Fargate
provider_slug: amazon-fargate
schema_file: json-schema/amazon-fargate-cluster-setting-schema.json
slug: amazon-fargate-cluster-setting
source_filename: amazon-fargate-cluster-setting-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-fargate/refs/heads/main/json-schema/amazon-fargate-cluster-setting-schema.json\",\n  \"title\": \"ClusterSetting\",\n  \"description\": \"A cluster setting\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Setting name\",\n      \"example\": \"containerInsights\"\n    },\n    \"value\": {\n      \"type\": \"string\",\n      \"description\": \"Setting value\",\n      \"example\": \"enabled\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-fargate/refs/heads/main/json-schema/amazon-fargate-cluster-setting-schema.json
tags:
- Compute
- Containers
- ECS
- EKS
- Microservices
- Serverless
title: ClusterSetting
---
