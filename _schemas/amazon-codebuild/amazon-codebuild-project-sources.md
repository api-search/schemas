---
description: ProjectSources schema from Amazon CodeBuild
layout: schema
name: ProjectSources
properties_list: []
provider_name: Amazon CodeBuild
provider_slug: amazon-codebuild
schema_file: json-schema/amazon-codebuild-project-sources-schema.json
slug: amazon-codebuild-project-sources
source_filename: amazon-codebuild-project-sources-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codebuild/refs/heads/main/json-schema/amazon-codebuild-project-sources-schema.json\",\n  \"title\": \"ProjectSources\",\n  \"description\": \"ProjectSources schema from Amazon CodeBuild\",\n  \"type\": \"array\",\n  \"items\": {\n    \"$ref\": \"#/components/schemas/ProjectSource\"\n  },\n  \"minItems\": 0,\n  \"maxItems\": 12\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codebuild/refs/heads/main/json-schema/amazon-codebuild-project-sources-schema.json
tags:
- Amazon
- CI/CD
- Build
- Continuous Integration
- DevOps
- Testing
title: ProjectSources
---
