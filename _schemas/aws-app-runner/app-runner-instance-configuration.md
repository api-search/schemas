---
description: InstanceConfiguration schema from AWS App Runner
layout: schema
name: InstanceConfiguration
properties_list:
- description: CPU units (e.g., 1024 for 1 vCPU, 256, 512, 1024, 2048, 4096).
  name: Cpu
  type: string
- description: Memory in MB (e.g., 2048 for 2 GB).
  name: Memory
  type: string
- description: ''
  name: InstanceRoleArn
  type: string
provider_name: AWS App Runner
provider_slug: aws-app-runner
schema_file: json-schema/app-runner-instance-configuration-schema.json
slug: app-runner-instance-configuration
tags:
- AWS
- CI/CD
- Containers
- Deployment
- Microservices
- Serverless
title: InstanceConfiguration
---
