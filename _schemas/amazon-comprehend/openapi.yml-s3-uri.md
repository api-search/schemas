---
description: S3Uri schema
layout: schema
name: S3Uri
properties_list: []
provider_name: Amazon Comprehend
provider_slug: amazon-comprehend
schema_file: json-schema/openapi.yml-s3-uri-schema.json
slug: openapi.yml-s3-uri
source_filename: openapi.yml-s3-uri-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-comprehend/refs/heads/main/json-schema/openapi.yml-s3-uri-schema.json\",\n  \"title\": \"S3Uri\",\n  \"description\": \"S3Uri schema\",\n  \"type\": \"string\",\n  \"pattern\": \"s3://[a-z0-9][\\\\.\\\\-a-z0-9]{1,61}[a-z0-9](/.*)?\",\n  \"maxLength\": 1024\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-comprehend/refs/heads/main/json-schema/openapi.yml-s3-uri-schema.json
tags:
- Machine Learning
- Natural Language Processing
- NLP
- Text Analysis
title: S3Uri
---
