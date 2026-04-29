---
description: InvalidateProjectCacheInput schema from Amazon CodeBuild
layout: schema
name: InvalidateProjectCacheInput
properties_list:
- description: ''
  name: projectName
  type: object
provider_name: Amazon CodeBuild
provider_slug: amazon-codebuild
schema_file: json-schema/amazon-codebuild-invalidate-project-cache-input-schema.json
slug: amazon-codebuild-invalidate-project-cache-input
source_filename: amazon-codebuild-invalidate-project-cache-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codebuild/refs/heads/main/json-schema/amazon-codebuild-invalidate-project-cache-input-schema.json\",\n  \"title\": \"InvalidateProjectCacheInput\",\n  \"description\": \"InvalidateProjectCacheInput schema from Amazon CodeBuild\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"projectName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NonEmptyString\"\n        },\n        {\n          \"description\": \"The name of the CodeBuild build project that the cache is reset for.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"projectName\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codebuild/refs/heads/main/json-schema/amazon-codebuild-invalidate-project-cache-input-schema.json
tags:
- Amazon
- AWS
- CI/CD
- Build
- Continuous Integration
- DevOps
- Testing
title: InvalidateProjectCacheInput
---
