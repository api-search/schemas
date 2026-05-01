---
description: RoleArn schema from Amazon CodePipeline
layout: schema
name: RoleArn
properties_list: []
provider_name: Amazon CodePipeline
provider_slug: amazon-codepipeline
schema_file: json-schema/amazon-codepipeline-role-arn-schema.json
slug: amazon-codepipeline-role-arn
source_filename: amazon-codepipeline-role-arn-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codepipeline/refs/heads/main/json-schema/amazon-codepipeline-role-arn-schema.json\",\n  \"title\": \"RoleArn\",\n  \"description\": \"RoleArn schema from Amazon CodePipeline\",\n  \"type\": \"string\",\n  \"pattern\": \"arn:aws(-[\\\\w]+)*:iam::[0-9]{12}:role/.*\",\n  \"maxLength\": 1024\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codepipeline/refs/heads/main/json-schema/amazon-codepipeline-role-arn-schema.json
tags:
- Amazon
- CI/CD
- Continuous Delivery
- DevOps
- Pipeline
- Release Automation
title: RoleArn
---
