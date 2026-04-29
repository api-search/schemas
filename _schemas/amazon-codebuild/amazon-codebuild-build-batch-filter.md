---
description: Specifies filters when retrieving batch builds.
layout: schema
name: BuildBatchFilter
properties_list:
- description: ''
  name: status
  type: object
provider_name: Amazon CodeBuild
provider_slug: amazon-codebuild
schema_file: json-schema/amazon-codebuild-build-batch-filter-schema.json
slug: amazon-codebuild-build-batch-filter
source_filename: amazon-codebuild-build-batch-filter-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codebuild/refs/heads/main/json-schema/amazon-codebuild-build-batch-filter-schema.json\",\n  \"title\": \"BuildBatchFilter\",\n  \"description\": \"Specifies filters when retrieving batch builds.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StatusType\"\n        },\n        {\n          \"description\": \"The status of the batch builds to retrieve. Only batch builds that have this status will be retrieved.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codebuild/refs/heads/main/json-schema/amazon-codebuild-build-batch-filter-schema.json
tags:
- Amazon
- AWS
- CI/CD
- Build
- Continuous Integration
- DevOps
- Testing
title: BuildBatchFilter
---
