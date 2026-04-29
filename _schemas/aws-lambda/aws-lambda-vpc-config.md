---
description: VPC connectivity settings for a Lambda function
layout: schema
name: VpcConfig
properties_list:
- description: A list of VPC subnet IDs
  name: SubnetIds
  type: array
- description: A list of VPC security group IDs
  name: SecurityGroupIds
  type: array
provider_name: AWS Lambda
provider_slug: aws-lambda
schema_file: json-schema/aws-lambda-vpc-config-schema.json
slug: aws-lambda-vpc-config
source_filename: aws-lambda-vpc-config-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"VpcConfig\",\n  \"type\": \"object\",\n  \"description\": \"VPC connectivity settings for a Lambda function\",\n  \"properties\": {\n    \"SubnetIds\": {\n      \"type\": \"array\",\n      \"description\": \"A list of VPC subnet IDs\"\n    },\n    \"SecurityGroupIds\": {\n      \"type\": \"array\",\n      \"description\": \"A list of VPC security group IDs\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-lambda/refs/heads/main/json-schema/aws-lambda-vpc-config-schema.json
tags: []
title: VpcConfig
---
