---
description: Location and destination information about the source code files provided with the project request. The source code is uploaded to the new project source repository after project creation.
layout: schema
name: Code
properties_list:
- description: ''
  name: source
  type: object
- description: ''
  name: destination
  type: object
provider_name: Amazon CodeStar
provider_slug: amazon-codestar
schema_file: json-schema/codestar-code-schema.json
slug: codestar-code
source_filename: codestar-code-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codestar/refs/heads/main/json-schema/codestar-code-schema.json\",\n  \"title\": \"Code\",\n  \"description\": \"Location and destination information about the source code files provided with the project request. The source code is uploaded to the new project source repository after project creation.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"source\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CodeSource\"\n        },\n        {\n          \"description\": \"The location where the source code files provided with the project request are stored. AWS CodeStar retrieves the files during project creation.\"\n        }\n      ]\n    },\n    \"destination\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CodeDestination\"\n        },\n        {\n          \"description\"\
  : \"The repository to be created in AWS CodeStar. Valid values are AWS CodeCommit or GitHub. After AWS CodeStar provisions the new repository, the source code files provided with the project request are placed in the repository.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"source\",\n    \"destination\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codestar/refs/heads/main/json-schema/codestar-code-schema.json
tags:
- Developer Tools
- DevOps
- Project Management
- Team Collaboration
title: Code
---
