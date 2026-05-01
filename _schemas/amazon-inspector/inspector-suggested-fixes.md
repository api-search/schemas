---
description: SuggestedFixes schema
layout: schema
name: SuggestedFixes
properties_list: []
provider_name: Amazon Inspector
provider_slug: amazon-inspector
schema_file: json-schema/inspector-suggested-fixes-schema.json
slug: inspector-suggested-fixes
source_filename: inspector-suggested-fixes-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-inspector/refs/heads/main/json-schema/inspector-suggested-fixes-schema.json\",\n  \"title\": \"SuggestedFixes\",\n  \"description\": \"SuggestedFixes schema\",\n  \"type\": \"array\",\n  \"items\": {\n    \"type\": \"object\",\n    \"properties\": {\n      \"code\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/SuggestedFixCodeString\"\n          },\n          {\n            \"description\": \"The fix's code.\"\n          }\n        ]\n      },\n      \"description\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/SuggestedFixDescriptionString\"\n          },\n          {\n            \"description\": \"The fix's description.\"\n          }\n        ]\n      }\n    },\n    \"description\": \"A suggested fix for a vulnerability in your Lambda function code.\"\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-inspector/refs/heads/main/json-schema/inspector-suggested-fixes-schema.json
tags:
- Compliance
- Container Security
- EC2
- Lambda
- Security
- Vulnerability Scanning
title: SuggestedFixes
---
