---
description: BuildBatches schema from Amazon CodeBuild
layout: schema
name: BuildBatches
properties_list: []
provider_name: Amazon CodeBuild
provider_slug: amazon-codebuild
schema_file: json-schema/amazon-codebuild-build-batches-schema.json
slug: amazon-codebuild-build-batches
source_filename: amazon-codebuild-build-batches-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codebuild/refs/heads/main/json-schema/amazon-codebuild-build-batches-schema.json\",\n  \"title\": \"BuildBatches\",\n  \"description\": \"BuildBatches schema from Amazon CodeBuild\",\n  \"type\": \"array\",\n  \"items\": {\n    \"$ref\": \"#/components/schemas/BuildBatch\"\n  },\n  \"minItems\": 0,\n  \"maxItems\": 100\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codebuild/refs/heads/main/json-schema/amazon-codebuild-build-batches-schema.json
tags:
- Amazon
- CI/CD
- Build
- Continuous Integration
- DevOps
- Testing
title: BuildBatches
---
