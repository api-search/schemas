---
description: CodeSnippetResultList schema
layout: schema
name: CodeSnippetResultList
properties_list: []
provider_name: Amazon Inspector
provider_slug: amazon-inspector
schema_file: json-schema/inspector-code-snippet-result-list-schema.json
slug: inspector-code-snippet-result-list
source_filename: inspector-code-snippet-result-list-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-inspector/refs/heads/main/json-schema/inspector-code-snippet-result-list-schema.json\",\n  \"title\": \"CodeSnippetResultList\",\n  \"description\": \"CodeSnippetResultList schema\",\n  \"type\": \"array\",\n  \"items\": {\n    \"type\": \"object\",\n    \"properties\": {\n      \"codeSnippet\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/CodeLineList\"\n          },\n          {\n            \"description\": \"Contains information on the retrieved code snippet.\"\n          }\n        ]\n      },\n      \"endLine\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/Integer\"\n          },\n          {\n            \"description\": \"The line number of the last line of a code snippet.\"\n          }\n        ]\n      },\n      \"findingArn\": {\n        \"allOf\": [\n\
  \          {\n            \"$ref\": \"#/components/schemas/FindingArn\"\n          },\n          {\n            \"description\": \"The ARN of a finding that the code snippet is associated with.\"\n          }\n        ]\n      },\n      \"startLine\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/Integer\"\n          },\n          {\n            \"description\": \"The line number of the first line of a code snippet.\"\n          }\n        ]\n      },\n      \"suggestedFixes\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/SuggestedFixes\"\n          },\n          {\n            \"description\": \"Details of a suggested code fix.\"\n          }\n        ]\n      }\n    },\n    \"description\": \"Contains information on a code snippet retrieved by Amazon Inspector from a code vulnerability finding.\"\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-inspector/refs/heads/main/json-schema/inspector-code-snippet-result-list-schema.json
tags:
- AWS
- Compliance
- Container Security
- EC2
- Lambda
- Security
- Vulnerability Scanning
title: CodeSnippetResultList
---
