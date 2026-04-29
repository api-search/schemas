---
description: Port mapping for a container
layout: schema
name: PortMapping
properties_list:
- description: Container port
  name: containerPort
  type: integer
- description: Host port
  name: hostPort
  type: integer
- description: Protocol
  name: protocol
  type: string
provider_name: Amazon Fargate
provider_slug: amazon-fargate
schema_file: json-schema/amazon-fargate-port-mapping-schema.json
slug: amazon-fargate-port-mapping
source_filename: amazon-fargate-port-mapping-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-fargate/refs/heads/main/json-schema/amazon-fargate-port-mapping-schema.json\",\n  \"title\": \"PortMapping\",\n  \"description\": \"Port mapping for a container\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"containerPort\": {\n      \"type\": \"integer\",\n      \"description\": \"Container port\",\n      \"example\": 80\n    },\n    \"hostPort\": {\n      \"type\": \"integer\",\n      \"description\": \"Host port\",\n      \"example\": 80\n    },\n    \"protocol\": {\n      \"type\": \"string\",\n      \"description\": \"Protocol\",\n      \"example\": \"tcp\",\n      \"enum\": [\n        \"tcp\",\n        \"udp\"\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-fargate/refs/heads/main/json-schema/amazon-fargate-port-mapping-schema.json
tags:
- AWS
- Compute
- Containers
- ECS
- EKS
- Microservices
- Serverless
title: PortMapping
---
