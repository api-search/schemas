---
description: BatchGetCodeSnippetRequest schema
layout: schema
name: BatchGetCodeSnippetRequest
properties_list:
- description: ''
  name: findingArns
  type: object
provider_name: Amazon Inspector
provider_slug: amazon-inspector
schema_file: json-schema/inspector-batch-get-code-snippet-request-schema.json
slug: inspector-batch-get-code-snippet-request
source_filename: inspector-batch-get-code-snippet-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-inspector/refs/heads/main/json-schema/inspector-batch-get-code-snippet-request-schema.json\",\n  \"title\": \"BatchGetCodeSnippetRequest\",\n  \"description\": \"BatchGetCodeSnippetRequest schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"findingArns\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BatchGetCodeSnippetRequestFindingArnsList\"\n        },\n        {\n          \"description\": \"An array of finding ARNs for the findings you want to retrieve code snippets from.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"findingArns\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-inspector/refs/heads/main/json-schema/inspector-batch-get-code-snippet-request-schema.json
tags:
- Compliance
- Container Security
- EC2
- Lambda
- Security
- Vulnerability Scanning
title: BatchGetCodeSnippetRequest
---
