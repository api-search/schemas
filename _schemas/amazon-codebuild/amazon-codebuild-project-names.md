---
description: ProjectNames schema from Amazon CodeBuild
layout: schema
name: ProjectNames
properties_list: []
provider_name: Amazon CodeBuild
provider_slug: amazon-codebuild
schema_file: json-schema/amazon-codebuild-project-names-schema.json
slug: amazon-codebuild-project-names
source_filename: amazon-codebuild-project-names-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codebuild/refs/heads/main/json-schema/amazon-codebuild-project-names-schema.json\",\n  \"title\": \"ProjectNames\",\n  \"description\": \"ProjectNames schema from Amazon CodeBuild\",\n  \"type\": \"array\",\n  \"items\": {\n    \"$ref\": \"#/components/schemas/NonEmptyString\"\n  },\n  \"minItems\": 1,\n  \"maxItems\": 100\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codebuild/refs/heads/main/json-schema/amazon-codebuild-project-names-schema.json
tags:
- Amazon
- CI/CD
- Build
- Continuous Integration
- DevOps
- Testing
title: ProjectNames
---
