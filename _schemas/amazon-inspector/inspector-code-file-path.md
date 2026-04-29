---
description: Contains information on where a code vulnerability is located in your Lambda function.
layout: schema
name: CodeFilePath
properties_list:
- description: ''
  name: endLine
  type: object
- description: ''
  name: fileName
  type: object
- description: ''
  name: filePath
  type: object
- description: ''
  name: startLine
  type: object
provider_name: Amazon Inspector
provider_slug: amazon-inspector
schema_file: json-schema/inspector-code-file-path-schema.json
slug: inspector-code-file-path
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-inspector/refs/heads/main/json-schema/inspector-code-file-path-schema.json\",\n  \"title\": \"CodeFilePath\",\n  \"description\": \"Contains information on where a code vulnerability is located in your Lambda function.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"endLine\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Integer\"\n        },\n        {\n          \"description\": \"The line number of the last line of code that a vulnerability was found in.\"\n        }\n      ]\n    },\n    \"fileName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NonEmptyString\"\n        },\n        {\n          \"description\": \"The name of the file the code vulnerability was found in.\"\n        }\n      ]\n    },\n    \"filePath\": {\n      \"allOf\": [\n        {\n          \"\
  $ref\": \"#/components/schemas/NonEmptyString\"\n        },\n        {\n          \"description\": \"The file path to the code that a vulnerability was found in.\"\n        }\n      ]\n    },\n    \"startLine\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Integer\"\n        },\n        {\n          \"description\": \"The line number of the first line of code that a vulnerability was found in.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"endLine\",\n    \"fileName\",\n    \"filePath\",\n    \"startLine\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-inspector/refs/heads/main/json-schema/inspector-code-file-path-schema.json
tags:
- AWS
- Compliance
- Container Security
- EC2
- Lambda
- Security
- Vulnerability Scanning
title: CodeFilePath
---
