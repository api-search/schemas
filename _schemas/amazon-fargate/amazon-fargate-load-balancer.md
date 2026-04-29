---
description: Load balancer configuration for a service
layout: schema
name: LoadBalancer
properties_list:
- description: Target group ARN
  name: targetGroupArn
  type: string
- description: Load balancer name
  name: loadBalancerName
  type: string
- description: Container name
  name: containerName
  type: string
- description: Container port
  name: containerPort
  type: integer
provider_name: Amazon Fargate
provider_slug: amazon-fargate
schema_file: json-schema/amazon-fargate-load-balancer-schema.json
slug: amazon-fargate-load-balancer
source_filename: amazon-fargate-load-balancer-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-fargate/refs/heads/main/json-schema/amazon-fargate-load-balancer-schema.json\",\n  \"title\": \"LoadBalancer\",\n  \"description\": \"Load balancer configuration for a service\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"targetGroupArn\": {\n      \"type\": \"string\",\n      \"description\": \"Target group ARN\",\n      \"example\": \"arn:aws:elasticloadbalancing:us-east-1:123456789012:targetgroup/my-tg/abc123\"\n    },\n    \"loadBalancerName\": {\n      \"type\": \"string\",\n      \"description\": \"Load balancer name\"\n    },\n    \"containerName\": {\n      \"type\": \"string\",\n      \"description\": \"Container name\",\n      \"example\": \"my-container\"\n    },\n    \"containerPort\": {\n      \"type\": \"integer\",\n      \"description\": \"Container port\",\n      \"example\": 80\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-fargate/refs/heads/main/json-schema/amazon-fargate-load-balancer-schema.json
tags:
- AWS
- Compute
- Containers
- ECS
- EKS
- Microservices
- Serverless
title: LoadBalancer
---
