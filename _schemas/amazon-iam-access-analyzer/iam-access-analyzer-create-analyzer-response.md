---
description: The response to the request to create an analyzer.
layout: schema
name: CreateAnalyzerResponse
properties_list:
- description: ''
  name: arn
  type: object
provider_name: Amazon IAM Access Analyzer
provider_slug: amazon-iam-access-analyzer
schema_file: json-schema/iam-access-analyzer-create-analyzer-response-schema.json
slug: iam-access-analyzer-create-analyzer-response
source_filename: iam-access-analyzer-create-analyzer-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iam-access-analyzer/refs/heads/main/json-schema/iam-access-analyzer-create-analyzer-response-schema.json\",\n  \"title\": \"CreateAnalyzerResponse\",\n  \"description\": \"The response to the request to create an analyzer.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"arn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AnalyzerArn\"\n        },\n        {\n          \"description\": \"The ARN of the analyzer that was created by the request.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iam-access-analyzer/refs/heads/main/json-schema/iam-access-analyzer-create-analyzer-response-schema.json
tags:
- Access Control
- Compliance
- IAM
- Policy Management
- Security
title: CreateAnalyzerResponse
---
