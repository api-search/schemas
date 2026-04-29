---
description: The Amazon S3 location where the toolchain template file provided with the project request is stored. AWS CodeStar retrieves the file during project creation.
layout: schema
name: ToolchainSource
properties_list:
- description: ''
  name: s3
  type: object
provider_name: Amazon CodeStar
provider_slug: amazon-codestar
schema_file: json-schema/codestar-toolchain-source-schema.json
slug: codestar-toolchain-source
source_filename: codestar-toolchain-source-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codestar/refs/heads/main/json-schema/codestar-toolchain-source-schema.json\",\n  \"title\": \"ToolchainSource\",\n  \"description\": \"The Amazon S3 location where the toolchain template file provided with the project request is stored. AWS CodeStar retrieves the file during project creation.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"s3\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/S3Location\"\n        },\n        {\n          \"description\": \"The Amazon S3 bucket where the toolchain template file provided with the project request is stored.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"s3\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codestar/refs/heads/main/json-schema/codestar-toolchain-source-schema.json
tags:
- AWS
- Developer Tools
- DevOps
- Project Management
- Team Collaboration
title: ToolchainSource
---
