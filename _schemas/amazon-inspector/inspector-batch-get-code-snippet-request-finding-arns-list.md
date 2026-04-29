---
description: BatchGetCodeSnippetRequestFindingArnsList schema
layout: schema
name: BatchGetCodeSnippetRequestFindingArnsList
properties_list: []
provider_name: Amazon Inspector
provider_slug: amazon-inspector
schema_file: json-schema/inspector-batch-get-code-snippet-request-finding-arns-list-schema.json
slug: inspector-batch-get-code-snippet-request-finding-arns-list
source_filename: inspector-batch-get-code-snippet-request-finding-arns-list-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-inspector/refs/heads/main/json-schema/inspector-batch-get-code-snippet-request-finding-arns-list-schema.json\",\n  \"title\": \"BatchGetCodeSnippetRequestFindingArnsList\",\n  \"description\": \"BatchGetCodeSnippetRequestFindingArnsList schema\",\n  \"type\": \"array\",\n  \"items\": {\n    \"type\": \"string\",\n    \"pattern\": \"^arn:(aws[a-zA-Z-]*)?:inspector2:[a-z]{2}(-gov)?-[a-z]+-\\\\d{1}:\\\\d{12}:finding/[a-f0-9]{32}$\",\n    \"minLength\": 1,\n    \"maxLength\": 100\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-inspector/refs/heads/main/json-schema/inspector-batch-get-code-snippet-request-finding-arns-list-schema.json
tags:
- AWS
- Compliance
- Container Security
- EC2
- Lambda
- Security
- Vulnerability Scanning
title: BatchGetCodeSnippetRequestFindingArnsList
---
