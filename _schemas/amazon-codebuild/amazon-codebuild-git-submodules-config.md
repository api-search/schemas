---
description: Information about the Git submodules configuration for an CodeBuild build project.
layout: schema
name: GitSubmodulesConfig
properties_list:
- description: ''
  name: fetchSubmodules
  type: object
provider_name: Amazon CodeBuild
provider_slug: amazon-codebuild
schema_file: json-schema/amazon-codebuild-git-submodules-config-schema.json
slug: amazon-codebuild-git-submodules-config
source_filename: amazon-codebuild-git-submodules-config-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codebuild/refs/heads/main/json-schema/amazon-codebuild-git-submodules-config-schema.json\",\n  \"title\": \"GitSubmodulesConfig\",\n  \"description\": \" Information about the Git submodules configuration for an CodeBuild build project. \",\n  \"type\": \"object\",\n  \"properties\": {\n    \"fetchSubmodules\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WrapperBoolean\"\n        },\n        {\n          \"description\": \" Set to true to fetch Git submodules for your CodeBuild build project. \"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"fetchSubmodules\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codebuild/refs/heads/main/json-schema/amazon-codebuild-git-submodules-config-schema.json
tags:
- Amazon
- CI/CD
- Build
- Continuous Integration
- DevOps
- Testing
title: GitSubmodulesConfig
---
