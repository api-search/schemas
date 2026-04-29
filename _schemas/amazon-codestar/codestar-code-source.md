---
description: The location where the source code files provided with the project request are stored. AWS CodeStar retrieves the files during project creation.
layout: schema
name: CodeSource
properties_list:
- description: ''
  name: s3
  type: object
provider_name: Amazon CodeStar
provider_slug: amazon-codestar
schema_file: json-schema/codestar-code-source-schema.json
slug: codestar-code-source
source_filename: codestar-code-source-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codestar/refs/heads/main/json-schema/codestar-code-source-schema.json\",\n  \"title\": \"CodeSource\",\n  \"description\": \"The location where the source code files provided with the project request are stored. AWS CodeStar retrieves the files during project creation.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"s3\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/S3Location\"\n        },\n        {\n          \"description\": \"Information about the Amazon S3 location where the source code files provided with the project request are stored. \"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"s3\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codestar/refs/heads/main/json-schema/codestar-code-source-schema.json
tags:
- AWS
- Developer Tools
- DevOps
- Project Management
- Team Collaboration
title: CodeSource
---
