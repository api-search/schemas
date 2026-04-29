---
description: The response to the request.
layout: schema
name: GetAnalyzerResponse
properties_list:
- description: ''
  name: analyzer
  type: object
provider_name: Amazon IAM Access Analyzer
provider_slug: amazon-iam-access-analyzer
schema_file: json-schema/iam-access-analyzer-get-analyzer-response-schema.json
slug: iam-access-analyzer-get-analyzer-response
source_filename: iam-access-analyzer-get-analyzer-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iam-access-analyzer/refs/heads/main/json-schema/iam-access-analyzer-get-analyzer-response-schema.json\",\n  \"title\": \"GetAnalyzerResponse\",\n  \"description\": \"The response to the request.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"analyzer\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AnalyzerSummary\"\n        },\n        {\n          \"description\": \"An <code>AnalyzerSummary</code> object that contains information about the analyzer.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"analyzer\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iam-access-analyzer/refs/heads/main/json-schema/iam-access-analyzer-get-analyzer-response-schema.json
tags:
- Access Control
- AWS
- Compliance
- IAM
- Policy Management
- Security
title: GetAnalyzerResponse
---
