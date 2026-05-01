---
description: A reference to a substring of a literal string in a JSON document.
layout: schema
name: Substring
properties_list:
- description: ''
  name: start
  type: object
- description: ''
  name: length
  type: object
provider_name: Amazon IAM Access Analyzer
provider_slug: amazon-iam-access-analyzer
schema_file: json-schema/iam-access-analyzer-substring-schema.json
slug: iam-access-analyzer-substring
source_filename: iam-access-analyzer-substring-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iam-access-analyzer/refs/heads/main/json-schema/iam-access-analyzer-substring-schema.json\",\n  \"title\": \"Substring\",\n  \"description\": \"A reference to a substring of a literal string in a JSON document.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"start\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Integer\"\n        },\n        {\n          \"description\": \"The start index of the substring, starting from 0.\"\n        }\n      ]\n    },\n    \"length\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Integer\"\n        },\n        {\n          \"description\": \"The length of the substring.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"start\",\n    \"length\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iam-access-analyzer/refs/heads/main/json-schema/iam-access-analyzer-substring-schema.json
tags:
- Access Control
- Compliance
- IAM
- Policy Management
- Security
title: Substring
---
