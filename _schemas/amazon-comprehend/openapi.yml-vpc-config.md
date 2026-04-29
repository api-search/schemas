---
description: Configuration parameters for an optional private Virtual Private Cloud (VPC) containing the resources you are using for the job. For more information, see <a href="https://docs.aws.amazon.com/vpc/latest/userguide/what-is-amazon-vpc.html">Amazon VPC</a>.
layout: schema
name: VpcConfig
properties_list:
- description: ''
  name: SecurityGroupIds
  type: object
- description: ''
  name: Subnets
  type: object
provider_name: Amazon Comprehend
provider_slug: amazon-comprehend
schema_file: json-schema/openapi.yml-vpc-config-schema.json
slug: openapi.yml-vpc-config
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-comprehend/refs/heads/main/json-schema/openapi.yml-vpc-config-schema.json\",\n  \"title\": \"VpcConfig\",\n  \"description\": \" Configuration parameters for an optional private Virtual Private Cloud (VPC) containing the resources you are using for the job. For more information, see <a href=\\\"https://docs.aws.amazon.com/vpc/latest/userguide/what-is-amazon-vpc.html\\\">Amazon VPC</a>. \",\n  \"type\": \"object\",\n  \"properties\": {\n    \"SecurityGroupIds\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SecurityGroupIds\"\n        },\n        {\n          \"description\": \"The ID number for a security group on an instance of your private VPC. Security groups on your VPC function serve as a virtual firewall to control inbound and outbound traffic and provides security for the resources that you\\u2019ll be\
  \ accessing on the VPC. This ID number is preceded by \\\"sg-\\\", for instance: \\\"sg-03b388029b0a285ea\\\". For more information, see <a href=\\\"https://docs.aws.amazon.com/vpc/latest/userguide/VPC_SecurityGroups.html\\\">Security Groups for your VPC</a>. \"\n        }\n      ]\n    },\n    \"Subnets\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Subnets\"\n        },\n        {\n          \"description\": \"The ID for each subnet being used in your private VPC. This subnet is a subset of the a range of IPv4 addresses used by the VPC and is specific to a given availability zone in the VPC\\u2019s Region. This ID number is preceded by \\\"subnet-\\\", for instance: \\\"subnet-04ccf456919e69055\\\". For more information, see <a href=\\\"https://docs.aws.amazon.com/vpc/latest/userguide/VPC_Subnets.html\\\">VPCs and Subnets</a>. \"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"SecurityGroupIds\",\n    \"Subnets\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-comprehend/refs/heads/main/json-schema/openapi.yml-vpc-config-schema.json
tags:
- AWS
- Machine Learning
- Natural Language Processing
- NLP
- Text Analysis
title: VpcConfig
---
