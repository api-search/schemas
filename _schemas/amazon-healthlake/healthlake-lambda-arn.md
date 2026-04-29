---
description: ''
layout: schema
name: LambdaArn
properties_list: []
provider_name: Amazon HealthLake
provider_slug: amazon-healthlake
schema_file: json-schema/healthlake-lambda-arn-schema.json
slug: healthlake-lambda-arn
source_filename: healthlake-lambda-arn-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-healthlake/refs/heads/main/json-schema/healthlake-lambda-arn-schema.json\",\n  \"title\": \"LambdaArn\",\n  \"type\": \"string\",\n  \"pattern\": \"arn:aws:lambda:[a-z]{2}-[a-z]+-\\\\d{1}:\\\\d{12}:function:[a-zA-Z0-9\\\\-_\\\\.]+(:(\\\\$LATEST|[a-zA-Z0-9\\\\-_]+))?\",\n  \"minLength\": 49,\n  \"maxLength\": 256\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-healthlake/refs/heads/main/json-schema/healthlake-lambda-arn-schema.json
tags:
- AWS
- FHIR
- Health Data
- Healthcare
- HIPAA
- Cloud Computing
title: LambdaArn
---
