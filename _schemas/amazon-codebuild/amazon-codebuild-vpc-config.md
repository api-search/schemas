---
description: Information about the VPC configuration that CodeBuild accesses.
layout: schema
name: VpcConfig
properties_list:
- description: ''
  name: vpcId
  type: object
- description: ''
  name: subnets
  type: object
- description: ''
  name: securityGroupIds
  type: object
provider_name: Amazon CodeBuild
provider_slug: amazon-codebuild
schema_file: json-schema/amazon-codebuild-vpc-config-schema.json
slug: amazon-codebuild-vpc-config
source_filename: amazon-codebuild-vpc-config-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codebuild/refs/heads/main/json-schema/amazon-codebuild-vpc-config-schema.json\",\n  \"title\": \"VpcConfig\",\n  \"description\": \"Information about the VPC configuration that CodeBuild accesses.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"vpcId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NonEmptyString\"\n        },\n        {\n          \"description\": \"The ID of the Amazon VPC.\"\n        }\n      ]\n    },\n    \"subnets\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Subnets\"\n        },\n        {\n          \"description\": \"A list of one or more subnet IDs in your Amazon VPC.\"\n        }\n      ]\n    },\n    \"securityGroupIds\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SecurityGroupIds\"\n        },\n       \
  \ {\n          \"description\": \"A list of one or more security groups IDs in your Amazon VPC.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codebuild/refs/heads/main/json-schema/amazon-codebuild-vpc-config-schema.json
tags:
- Amazon
- AWS
- CI/CD
- Build
- Continuous Integration
- DevOps
- Testing
title: VpcConfig
---
