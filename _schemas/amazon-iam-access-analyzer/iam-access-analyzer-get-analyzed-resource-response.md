---
description: The response to the request.
layout: schema
name: GetAnalyzedResourceResponse
properties_list:
- description: ''
  name: resource
  type: object
provider_name: Amazon IAM Access Analyzer
provider_slug: amazon-iam-access-analyzer
schema_file: json-schema/iam-access-analyzer-get-analyzed-resource-response-schema.json
slug: iam-access-analyzer-get-analyzed-resource-response
source_filename: iam-access-analyzer-get-analyzed-resource-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iam-access-analyzer/refs/heads/main/json-schema/iam-access-analyzer-get-analyzed-resource-response-schema.json\",\n  \"title\": \"GetAnalyzedResourceResponse\",\n  \"description\": \"The response to the request.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"resource\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AnalyzedResource\"\n        },\n        {\n          \"description\": \"An <code>AnalyzedResource</code> object that contains information that IAM Access Analyzer found when it analyzed the resource.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iam-access-analyzer/refs/heads/main/json-schema/iam-access-analyzer-get-analyzed-resource-response-schema.json
tags:
- Access Control
- Compliance
- IAM
- Policy Management
- Security
title: GetAnalyzedResourceResponse
---
