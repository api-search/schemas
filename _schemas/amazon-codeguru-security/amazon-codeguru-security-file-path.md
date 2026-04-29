---
description: Information about the location of security vulnerabilities that Amazon CodeGuru Security detected in your code.
layout: schema
name: FilePath
properties_list:
- description: ''
  name: codeSnippet
  type: object
- description: ''
  name: endLine
  type: object
- description: ''
  name: name
  type: object
- description: ''
  name: path
  type: object
- description: ''
  name: startLine
  type: object
provider_name: Amazon CodeGuru Security
provider_slug: amazon-codeguru-security
schema_file: json-schema/amazon-codeguru-security-file-path-schema.json
slug: amazon-codeguru-security-file-path
source_filename: amazon-codeguru-security-file-path-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codeguru-security/refs/heads/main/json-schema/amazon-codeguru-security-file-path-schema.json\",\n  \"title\": \"FilePath\",\n  \"description\": \"Information about the location of security vulnerabilities that Amazon CodeGuru Security detected in your code.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"codeSnippet\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CodeSnippet\"\n        },\n        {\n          \"description\": \"A list of <code>CodeLine</code> objects that describe where the security vulnerability appears in your code.\"\n        }\n      ]\n    },\n    \"endLine\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Integer\"\n        },\n        {\n          \"description\": \"The last line number of the code snippet where the security vulnerability appears\
  \ in your code.\"\n        }\n      ]\n    },\n    \"name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The name of the file.\"\n        }\n      ]\n    },\n    \"path\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The path to the resource with the security vulnerability.\"\n        }\n      ]\n    },\n    \"startLine\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Integer\"\n        },\n        {\n          \"description\": \"The first line number of the code snippet where the security vulnerability appears in your code.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codeguru-security/refs/heads/main/json-schema/amazon-codeguru-security-file-path-schema.json
tags:
- Amazon
- AWS
- Security
- SAST
- Code Analysis
- DevSecOps
- Developer Tools
title: FilePath
---
