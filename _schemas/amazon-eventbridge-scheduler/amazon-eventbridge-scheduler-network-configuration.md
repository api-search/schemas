---
description: Specifies the network configuration for an ECS task.
layout: schema
name: NetworkConfiguration
properties_list:
- description: ''
  name: awsvpcConfiguration
  type: object
provider_name: Amazon EventBridge Scheduler
provider_slug: amazon-eventbridge-scheduler
schema_file: json-schema/amazon-eventbridge-scheduler-network-configuration-schema.json
slug: amazon-eventbridge-scheduler-network-configuration
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-eventbridge-scheduler/refs/heads/main/json-schema/amazon-eventbridge-scheduler-network-configuration-schema.json\",\n  \"title\": \"NetworkConfiguration\",\n  \"description\": \"Specifies the network configuration for an ECS task.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"awsvpcConfiguration\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AwsVpcConfiguration\"\n        },\n        {\n          \"description\": \"Specifies the Amazon VPC subnets and security groups for the task, and whether a public IP address is to be used. This structure is relevant only for ECS tasks that use the awsvpc network mode.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-eventbridge-scheduler/refs/heads/main/json-schema/amazon-eventbridge-scheduler-network-configuration-schema.json
tags:
- Amazon Web Services
- AWS
- Cron
- Event-Driven
- Scheduling
- Serverless
title: NetworkConfiguration
---
