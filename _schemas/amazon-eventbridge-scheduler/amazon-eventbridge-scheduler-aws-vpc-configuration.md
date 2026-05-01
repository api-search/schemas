---
description: This structure specifies the VPC subnets and security groups for the task, and whether a public IP address is to be used. This structure is relevant only for ECS tasks that use the awsvpc network mode.
layout: schema
name: AwsVpcConfiguration
properties_list:
- description: ''
  name: AssignPublicIp
  type: object
- description: ''
  name: SecurityGroups
  type: object
- description: ''
  name: Subnets
  type: object
provider_name: Amazon EventBridge Scheduler
provider_slug: amazon-eventbridge-scheduler
schema_file: json-schema/amazon-eventbridge-scheduler-aws-vpc-configuration-schema.json
slug: amazon-eventbridge-scheduler-aws-vpc-configuration
source_filename: amazon-eventbridge-scheduler-aws-vpc-configuration-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-eventbridge-scheduler/refs/heads/main/json-schema/amazon-eventbridge-scheduler-aws-vpc-configuration-schema.json\",\n  \"title\": \"AwsVpcConfiguration\",\n  \"description\": \"This structure specifies the VPC subnets and security groups for the task, and whether a public IP address is to be used. This structure is relevant only for ECS tasks that use the awsvpc network mode.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AssignPublicIp\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AssignPublicIp\"\n        },\n        {\n          \"description\": \"Specifies whether the task's elastic network interface receives a public IP address. You can specify <code>ENABLED</code> only when <code>LaunchType</code> in <code>EcsParameters</code> is set to <code>FARGATE</code>.\"\n        }\n      ]\n    },\n\
  \    \"SecurityGroups\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SecurityGroups\"\n        },\n        {\n          \"description\": \"Specifies the security groups associated with the task. These security groups must all be in the same VPC. You can specify as many as five security groups. If you do not specify a security group, the default security group for the VPC is used.\"\n        }\n      ]\n    },\n    \"Subnets\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Subnets\"\n        },\n        {\n          \"description\": \"Specifies the subnets associated with the task. These subnets must all be in the same VPC. You can specify as many as 16 subnets.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Subnets\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-eventbridge-scheduler/refs/heads/main/json-schema/amazon-eventbridge-scheduler-aws-vpc-configuration-schema.json
tags:
- Amazon Web Services
- Cron
- Event-Driven
- Scheduling
- Serverless
title: AwsVpcConfiguration
---
