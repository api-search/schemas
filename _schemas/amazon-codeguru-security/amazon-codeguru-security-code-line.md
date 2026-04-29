---
description: The line of code where a finding was detected.
layout: schema
name: CodeLine
properties_list:
- description: ''
  name: content
  type: object
- description: ''
  name: number
  type: object
provider_name: Amazon CodeGuru Security
provider_slug: amazon-codeguru-security
schema_file: json-schema/amazon-codeguru-security-code-line-schema.json
slug: amazon-codeguru-security-code-line
source_filename: amazon-codeguru-security-code-line-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codeguru-security/refs/heads/main/json-schema/amazon-codeguru-security-code-line-schema.json\",\n  \"title\": \"CodeLine\",\n  \"description\": \"The line of code where a finding was detected.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"content\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The code that contains a vulnerability.\"\n        }\n      ]\n    },\n    \"number\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Integer\"\n        },\n        {\n          \"description\": \"The code line number.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codeguru-security/refs/heads/main/json-schema/amazon-codeguru-security-code-line-schema.json
tags:
- Amazon
- AWS
- Security
- SAST
- Code Analysis
- DevSecOps
- Developer Tools
title: CodeLine
---
