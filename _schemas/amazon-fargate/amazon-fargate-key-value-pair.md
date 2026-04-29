---
description: A key-value pair
layout: schema
name: KeyValuePair
properties_list:
- description: Key name
  name: name
  type: string
- description: Key value
  name: value
  type: string
provider_name: Amazon Fargate
provider_slug: amazon-fargate
schema_file: json-schema/amazon-fargate-key-value-pair-schema.json
slug: amazon-fargate-key-value-pair
source_filename: amazon-fargate-key-value-pair-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-fargate/refs/heads/main/json-schema/amazon-fargate-key-value-pair-schema.json\",\n  \"title\": \"KeyValuePair\",\n  \"description\": \"A key-value pair\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Key name\",\n      \"example\": \"LOG_LEVEL\"\n    },\n    \"value\": {\n      \"type\": \"string\",\n      \"description\": \"Key value\",\n      \"example\": \"INFO\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-fargate/refs/heads/main/json-schema/amazon-fargate-key-value-pair-schema.json
tags:
- AWS
- Compute
- Containers
- ECS
- EKS
- Microservices
- Serverless
title: KeyValuePair
---
