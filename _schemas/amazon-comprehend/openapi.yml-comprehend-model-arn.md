---
description: ComprehendModelArn schema
layout: schema
name: ComprehendModelArn
properties_list: []
provider_name: Amazon Comprehend
provider_slug: amazon-comprehend
schema_file: json-schema/openapi.yml-comprehend-model-arn-schema.json
slug: openapi.yml-comprehend-model-arn
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-comprehend/refs/heads/main/json-schema/openapi.yml-comprehend-model-arn-schema.json\",\n  \"title\": \"ComprehendModelArn\",\n  \"description\": \"ComprehendModelArn schema\",\n  \"type\": \"string\",\n  \"pattern\": \"arn:aws(-[^:]+)?:comprehend:[a-zA-Z0-9-]*:[0-9]{12}:(document-classifier|entity-recognizer)/[a-zA-Z0-9](-*[a-zA-Z0-9])*(/version/[a-zA-Z0-9](-*[a-zA-Z0-9])*)?\",\n  \"maxLength\": 256\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-comprehend/refs/heads/main/json-schema/openapi.yml-comprehend-model-arn-schema.json
tags:
- AWS
- Machine Learning
- Natural Language Processing
- NLP
- Text Analysis
title: ComprehendModelArn
---
