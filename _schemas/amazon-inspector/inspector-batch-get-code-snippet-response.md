---
description: BatchGetCodeSnippetResponse schema
layout: schema
name: BatchGetCodeSnippetResponse
properties_list:
- description: ''
  name: codeSnippetResults
  type: object
- description: ''
  name: errors
  type: object
provider_name: Amazon Inspector
provider_slug: amazon-inspector
schema_file: json-schema/inspector-batch-get-code-snippet-response-schema.json
slug: inspector-batch-get-code-snippet-response
source_filename: inspector-batch-get-code-snippet-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-inspector/refs/heads/main/json-schema/inspector-batch-get-code-snippet-response-schema.json\",\n  \"title\": \"BatchGetCodeSnippetResponse\",\n  \"description\": \"BatchGetCodeSnippetResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"codeSnippetResults\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CodeSnippetResultList\"\n        },\n        {\n          \"description\": \"The retrieved code snippets associated with the provided finding ARNs.\"\n        }\n      ]\n    },\n    \"errors\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CodeSnippetErrorList\"\n        },\n        {\n          \"description\": \"Any errors Amazon Inspector encountered while trying to retrieve the requested code snippets.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-inspector/refs/heads/main/json-schema/inspector-batch-get-code-snippet-response-schema.json
tags:
- AWS
- Compliance
- Container Security
- EC2
- Lambda
- Security
- Vulnerability Scanning
title: BatchGetCodeSnippetResponse
---
