---
description: The VPC security groups and subnets that are attached to an AWS Lambda function. For more information, see <a href="https://docs.aws.amazon.com/lambda/latest/dg/configuration-vpc.html">VPC Settings</a>.
layout: schema
name: LambdaVpcConfig
properties_list:
- description: ''
  name: securityGroupIds
  type: object
- description: ''
  name: subnetIds
  type: object
- description: ''
  name: vpcId
  type: object
provider_name: Amazon Inspector
provider_slug: amazon-inspector
schema_file: json-schema/inspector-lambda-vpc-config-schema.json
slug: inspector-lambda-vpc-config
source_filename: inspector-lambda-vpc-config-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-inspector/refs/heads/main/json-schema/inspector-lambda-vpc-config-schema.json\",\n  \"title\": \"LambdaVpcConfig\",\n  \"description\": \"The VPC security groups and subnets that are attached to an AWS Lambda function. For more information, see <a href=\\\"https://docs.aws.amazon.com/lambda/latest/dg/configuration-vpc.html\\\">VPC Settings</a>.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"securityGroupIds\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SecurityGroupIdList\"\n        },\n        {\n          \"description\": \"The VPC security groups and subnets that are attached to an AWS Lambda function. For more information, see <a href=\\\"https://docs.aws.amazon.com/lambda/latest/dg/configuration-vpc.html\\\">VPC Settings</a>.\"\n        }\n      ]\n    },\n    \"subnetIds\": {\n      \"allOf\"\
  : [\n        {\n          \"$ref\": \"#/components/schemas/SubnetIdList\"\n        },\n        {\n          \"description\": \"A list of VPC subnet IDs.\"\n        }\n      ]\n    },\n    \"vpcId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/VpcId\"\n        },\n        {\n          \"description\": \"The ID of the VPC.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-inspector/refs/heads/main/json-schema/inspector-lambda-vpc-config-schema.json
tags:
- Compliance
- Container Security
- EC2
- Lambda
- Security
- Vulnerability Scanning
title: LambdaVpcConfig
---
