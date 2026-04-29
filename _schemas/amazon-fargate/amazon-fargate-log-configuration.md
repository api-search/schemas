---
description: Log configuration for a container
layout: schema
name: LogConfiguration
properties_list:
- description: Log driver
  name: logDriver
  type: string
- description: Log driver options
  name: options
  type: object
provider_name: Amazon Fargate
provider_slug: amazon-fargate
schema_file: json-schema/amazon-fargate-log-configuration-schema.json
slug: amazon-fargate-log-configuration
source_filename: amazon-fargate-log-configuration-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-fargate/refs/heads/main/json-schema/amazon-fargate-log-configuration-schema.json\",\n  \"title\": \"LogConfiguration\",\n  \"description\": \"Log configuration for a container\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"logDriver\": {\n      \"type\": \"string\",\n      \"description\": \"Log driver\",\n      \"example\": \"awslogs\",\n      \"enum\": [\n        \"json-file\",\n        \"syslog\",\n        \"journald\",\n        \"gelf\",\n        \"fluentd\",\n        \"awslogs\",\n        \"splunk\",\n        \"awsfirelens\"\n      ]\n    },\n    \"options\": {\n      \"type\": \"object\",\n      \"description\": \"Log driver options\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-fargate/refs/heads/main/json-schema/amazon-fargate-log-configuration-schema.json
tags:
- AWS
- Compute
- Containers
- ECS
- EKS
- Microservices
- Serverless
title: LogConfiguration
---
