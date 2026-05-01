---
description: CodeLineList schema
layout: schema
name: CodeLineList
properties_list: []
provider_name: Amazon Inspector
provider_slug: amazon-inspector
schema_file: json-schema/inspector-code-line-list-schema.json
slug: inspector-code-line-list
source_filename: inspector-code-line-list-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-inspector/refs/heads/main/json-schema/inspector-code-line-list-schema.json\",\n  \"title\": \"CodeLineList\",\n  \"description\": \"CodeLineList schema\",\n  \"type\": \"array\",\n  \"items\": {\n    \"type\": \"object\",\n    \"required\": [\n      \"content\",\n      \"lineNumber\"\n    ],\n    \"properties\": {\n      \"content\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/CodeLineContentString\"\n          },\n          {\n            \"description\": \"The content of a line of code\"\n          }\n        ]\n      },\n      \"lineNumber\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/Integer\"\n          },\n          {\n            \"description\": \"The line number that a section of code is located at.\"\n          }\n        ]\n      }\n    },\n    \"description\"\
  : \"Contains information on the lines of code associated with a code snippet.\"\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-inspector/refs/heads/main/json-schema/inspector-code-line-list-schema.json
tags:
- Compliance
- Container Security
- EC2
- Lambda
- Security
- Vulnerability Scanning
title: CodeLineList
---
