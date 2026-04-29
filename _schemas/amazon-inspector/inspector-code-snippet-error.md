---
description: Contains information about any errors encountered while trying to retrieve a code snippet.
layout: schema
name: CodeSnippetError
properties_list:
- description: ''
  name: errorCode
  type: object
- description: ''
  name: errorMessage
  type: object
- description: ''
  name: findingArn
  type: object
provider_name: Amazon Inspector
provider_slug: amazon-inspector
schema_file: json-schema/inspector-code-snippet-error-schema.json
slug: inspector-code-snippet-error
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-inspector/refs/heads/main/json-schema/inspector-code-snippet-error-schema.json\",\n  \"title\": \"CodeSnippetError\",\n  \"description\": \"Contains information about any errors encountered while trying to retrieve a code snippet.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"errorCode\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CodeSnippetErrorCode\"\n        },\n        {\n          \"description\": \"The error code for the error that prevented a code snippet from being retrieved.\"\n        }\n      ]\n    },\n    \"errorMessage\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NonEmptyString\"\n        },\n        {\n          \"description\": \"The error message received when Amazon Inspector failed to retrieve a code snippet.\"\n        }\n      ]\n    },\n\
  \    \"findingArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FindingArn\"\n        },\n        {\n          \"description\": \"The ARN of the finding that a code snippet couldn't be retrieved for.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"errorCode\",\n    \"errorMessage\",\n    \"findingArn\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-inspector/refs/heads/main/json-schema/inspector-code-snippet-error-schema.json
tags:
- AWS
- Compliance
- Container Security
- EC2
- Lambda
- Security
- Vulnerability Scanning
title: CodeSnippetError
---
