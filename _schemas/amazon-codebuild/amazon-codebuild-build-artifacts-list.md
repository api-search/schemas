---
description: BuildArtifactsList schema from Amazon CodeBuild
layout: schema
name: BuildArtifactsList
properties_list: []
provider_name: Amazon CodeBuild
provider_slug: amazon-codebuild
schema_file: json-schema/amazon-codebuild-build-artifacts-list-schema.json
slug: amazon-codebuild-build-artifacts-list
source_filename: amazon-codebuild-build-artifacts-list-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codebuild/refs/heads/main/json-schema/amazon-codebuild-build-artifacts-list-schema.json\",\n  \"title\": \"BuildArtifactsList\",\n  \"description\": \"BuildArtifactsList schema from Amazon CodeBuild\",\n  \"type\": \"array\",\n  \"items\": {\n    \"$ref\": \"#/components/schemas/BuildArtifacts\"\n  },\n  \"minItems\": 0,\n  \"maxItems\": 12\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codebuild/refs/heads/main/json-schema/amazon-codebuild-build-artifacts-list-schema.json
tags:
- Amazon
- AWS
- CI/CD
- Build
- Continuous Integration
- DevOps
- Testing
title: BuildArtifactsList
---
