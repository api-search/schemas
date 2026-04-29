---
description: ComprehendArn schema
layout: schema
name: ComprehendArn
properties_list: []
provider_name: Amazon Comprehend
provider_slug: amazon-comprehend
schema_file: json-schema/openapi.yml-comprehend-arn-schema.json
slug: openapi.yml-comprehend-arn
source_filename: openapi.yml-comprehend-arn-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-comprehend/refs/heads/main/json-schema/openapi.yml-comprehend-arn-schema.json\",\n  \"title\": \"ComprehendArn\",\n  \"description\": \"ComprehendArn schema\",\n  \"type\": \"string\",\n  \"pattern\": \"arn:aws(-[^:]+)?:comprehend:[a-zA-Z0-9-]*:[0-9]{12}:[a-zA-Z0-9-]{1,64}/[a-zA-Z0-9](-*[a-zA-Z0-9])*((/dataset/[a-zA-Z0-9](-*[a-zA-Z0-9])*)|(/version/[a-zA-Z0-9](-*[a-zA-Z0-9])*))?\",\n  \"maxLength\": 256\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-comprehend/refs/heads/main/json-schema/openapi.yml-comprehend-arn-schema.json
tags:
- AWS
- Machine Learning
- Natural Language Processing
- NLP
- Text Analysis
title: ComprehendArn
---
