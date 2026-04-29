---
description: This structure specifies the network configuration for an Amazon ECS task.
layout: schema
name: NetworkConfiguration
properties_list:
- description: ''
  name: awsvpcConfiguration
  type: object
provider_name: Amazon EventBridge Pipes
provider_slug: amazon-eventbridge-pipes
schema_file: json-schema/amazon-eventbridge-pipes-network-configuration-schema.json
slug: amazon-eventbridge-pipes-network-configuration
source_filename: amazon-eventbridge-pipes-network-configuration-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-eventbridge-pipes/refs/heads/main/json-schema/amazon-eventbridge-pipes-network-configuration-schema.json\",\n  \"title\": \"NetworkConfiguration\",\n  \"description\": \"This structure specifies the network configuration for an Amazon ECS task.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"awsvpcConfiguration\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AwsVpcConfiguration\"\n        },\n        {\n          \"description\": \"Use this structure to specify the VPC subnets and security groups for the task, and whether a public IP address is to be used. This structure is relevant only for ECS tasks that use the <code>awsvpc</code> network mode.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-eventbridge-pipes/refs/heads/main/json-schema/amazon-eventbridge-pipes-network-configuration-schema.json
tags:
- Amazon Web Services
- AWS
- Event-Driven
- Integration
- Messaging
- Serverless
title: NetworkConfiguration
---
