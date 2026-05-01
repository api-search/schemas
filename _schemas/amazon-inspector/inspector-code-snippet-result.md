---
description: Contains information on a code snippet retrieved by Amazon Inspector from a code vulnerability finding.
layout: schema
name: CodeSnippetResult
properties_list:
- description: ''
  name: codeSnippet
  type: object
- description: ''
  name: endLine
  type: object
- description: ''
  name: findingArn
  type: object
- description: ''
  name: startLine
  type: object
- description: ''
  name: suggestedFixes
  type: object
provider_name: Amazon Inspector
provider_slug: amazon-inspector
schema_file: json-schema/inspector-code-snippet-result-schema.json
slug: inspector-code-snippet-result
source_filename: inspector-code-snippet-result-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-inspector/refs/heads/main/json-schema/inspector-code-snippet-result-schema.json\",\n  \"title\": \"CodeSnippetResult\",\n  \"description\": \"Contains information on a code snippet retrieved by Amazon Inspector from a code vulnerability finding.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"codeSnippet\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CodeLineList\"\n        },\n        {\n          \"description\": \"Contains information on the retrieved code snippet.\"\n        }\n      ]\n    },\n    \"endLine\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Integer\"\n        },\n        {\n          \"description\": \"The line number of the last line of a code snippet.\"\n        }\n      ]\n    },\n    \"findingArn\": {\n      \"allOf\": [\n        {\n          \"\
  $ref\": \"#/components/schemas/FindingArn\"\n        },\n        {\n          \"description\": \"The ARN of a finding that the code snippet is associated with.\"\n        }\n      ]\n    },\n    \"startLine\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Integer\"\n        },\n        {\n          \"description\": \"The line number of the first line of a code snippet.\"\n        }\n      ]\n    },\n    \"suggestedFixes\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SuggestedFixes\"\n        },\n        {\n          \"description\": \"Details of a suggested code fix.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-inspector/refs/heads/main/json-schema/inspector-code-snippet-result-schema.json
tags:
- Compliance
- Container Security
- EC2
- Lambda
- Security
- Vulnerability Scanning
title: CodeSnippetResult
---
