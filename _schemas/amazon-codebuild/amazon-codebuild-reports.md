---
description: Reports schema from Amazon CodeBuild
layout: schema
name: Reports
properties_list: []
provider_name: Amazon CodeBuild
provider_slug: amazon-codebuild
schema_file: json-schema/amazon-codebuild-reports-schema.json
slug: amazon-codebuild-reports
source_filename: amazon-codebuild-reports-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codebuild/refs/heads/main/json-schema/amazon-codebuild-reports-schema.json\",\n  \"title\": \"Reports\",\n  \"description\": \"Reports schema from Amazon CodeBuild\",\n  \"type\": \"array\",\n  \"items\": {\n    \"$ref\": \"#/components/schemas/Report\"\n  },\n  \"minItems\": 1,\n  \"maxItems\": 100\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codebuild/refs/heads/main/json-schema/amazon-codebuild-reports-schema.json
tags:
- Amazon
- CI/CD
- Build
- Continuous Integration
- DevOps
- Testing
title: Reports
---
