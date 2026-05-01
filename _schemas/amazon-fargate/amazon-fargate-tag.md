---
description: A tag applied to an ECS resource
layout: schema
name: Tag
properties_list:
- description: The tag key
  name: key
  type: string
- description: The tag value
  name: value
  type: string
provider_name: Amazon Fargate
provider_slug: amazon-fargate
schema_file: json-schema/amazon-fargate-tag-schema.json
slug: amazon-fargate-tag
source_filename: amazon-fargate-tag-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-fargate/refs/heads/main/json-schema/amazon-fargate-tag-schema.json\",\n  \"title\": \"Tag\",\n  \"description\": \"A tag applied to an ECS resource\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"key\": {\n      \"type\": \"string\",\n      \"description\": \"The tag key\",\n      \"example\": \"Environment\"\n    },\n    \"value\": {\n      \"type\": \"string\",\n      \"description\": \"The tag value\",\n      \"example\": \"production\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-fargate/refs/heads/main/json-schema/amazon-fargate-tag-schema.json
tags:
- Compute
- Containers
- ECS
- EKS
- Microservices
- Serverless
title: Tag
---
