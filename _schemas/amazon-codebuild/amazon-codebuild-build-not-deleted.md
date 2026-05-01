---
description: Information about a build that could not be successfully deleted.
layout: schema
name: BuildNotDeleted
properties_list:
- description: ''
  name: id
  type: object
- description: ''
  name: statusCode
  type: object
provider_name: Amazon CodeBuild
provider_slug: amazon-codebuild
schema_file: json-schema/amazon-codebuild-build-not-deleted-schema.json
slug: amazon-codebuild-build-not-deleted
source_filename: amazon-codebuild-build-not-deleted-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codebuild/refs/heads/main/json-schema/amazon-codebuild-build-not-deleted-schema.json\",\n  \"title\": \"BuildNotDeleted\",\n  \"description\": \"Information about a build that could not be successfully deleted.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NonEmptyString\"\n        },\n        {\n          \"description\": \"The ID of the build that could not be successfully deleted.\"\n        }\n      ]\n    },\n    \"statusCode\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"Additional information about the build that could not be successfully deleted.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codebuild/refs/heads/main/json-schema/amazon-codebuild-build-not-deleted-schema.json
tags:
- Amazon
- CI/CD
- Build
- Continuous Integration
- DevOps
- Testing
title: BuildNotDeleted
---
