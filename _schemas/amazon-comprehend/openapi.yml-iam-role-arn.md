---
description: IamRoleArn schema
layout: schema
name: IamRoleArn
properties_list: []
provider_name: Amazon Comprehend
provider_slug: amazon-comprehend
schema_file: json-schema/openapi.yml-iam-role-arn-schema.json
slug: openapi.yml-iam-role-arn
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-comprehend/refs/heads/main/json-schema/openapi.yml-iam-role-arn-schema.json\",\n  \"title\": \"IamRoleArn\",\n  \"description\": \"IamRoleArn schema\",\n  \"type\": \"string\",\n  \"pattern\": \"arn:aws(-[^:]+)?:iam::[0-9]{12}:role/.+\",\n  \"minLength\": 20,\n  \"maxLength\": 2048\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-comprehend/refs/heads/main/json-schema/openapi.yml-iam-role-arn-schema.json
tags:
- AWS
- Machine Learning
- Natural Language Processing
- NLP
- Text Analysis
title: IamRoleArn
---
