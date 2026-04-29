---
description: ''
layout: schema
name: LoadBalancer
properties_list:
- description: The full ARN of the Elastic Load Balancing target group.
  name: targetGroupArn
  type: string
- description: The name of the load balancer (Classic Load Balancer only).
  name: loadBalancerName
  type: string
- description: The name of the container to associate with the load balancer.
  name: containerName
  type: string
- description: The port on the container to associate with the load balancer.
  name: containerPort
  type: integer
provider_name: Amazon ECS
provider_slug: amazon-ecs
schema_file: json-schema/amazon-ecs-load-balancer-schema.json
slug: amazon-ecs-load-balancer
source_filename: amazon-ecs-load-balancer-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"LoadBalancer\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"targetGroupArn\": {\n      \"type\": \"string\",\n      \"description\": \"The full ARN of the Elastic Load Balancing target group.\"\n    },\n    \"loadBalancerName\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the load balancer (Classic Load Balancer only).\"\n    },\n    \"containerName\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the container to associate with the load balancer.\"\n    },\n    \"containerPort\": {\n      \"type\": \"integer\",\n      \"description\": \"The port on the container to associate with the load balancer.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ecs/refs/heads/main/json-schema/amazon-ecs-load-balancer-schema.json
tags:
- Amazon
- Aws
- Containers
- Docker
- Ecs
- Orchestration
title: LoadBalancer
---
