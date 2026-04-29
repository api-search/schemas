---
description: VPC connectivity details returned by Lambda
layout: schema
name: VpcConfigResponse
properties_list:
- description: ''
  name: SubnetIds
  type: array
- description: ''
  name: SecurityGroupIds
  type: array
- description: The VPC ID
  name: VpcId
  type: string
provider_name: AWS Lambda
provider_slug: aws-lambda
schema_file: json-schema/aws-lambda-vpc-config-response-schema.json
slug: aws-lambda-vpc-config-response
source_filename: aws-lambda-vpc-config-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"VpcConfigResponse\",\n  \"type\": \"object\",\n  \"description\": \"VPC connectivity details returned by Lambda\",\n  \"properties\": {\n    \"SubnetIds\": {\n      \"type\": \"array\"\n    },\n    \"SecurityGroupIds\": {\n      \"type\": \"array\"\n    },\n    \"VpcId\": {\n      \"type\": \"string\",\n      \"description\": \"The VPC ID\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-lambda/refs/heads/main/json-schema/aws-lambda-vpc-config-response-schema.json
tags: []
title: VpcConfigResponse
---
