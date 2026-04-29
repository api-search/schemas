---
description: BatchDeleteBuildsOutput schema from Amazon CodeBuild
layout: schema
name: BatchDeleteBuildsOutput
properties_list:
- description: ''
  name: buildsDeleted
  type: object
- description: ''
  name: buildsNotDeleted
  type: object
provider_name: Amazon CodeBuild
provider_slug: amazon-codebuild
schema_file: json-schema/amazon-codebuild-batch-delete-builds-output-schema.json
slug: amazon-codebuild-batch-delete-builds-output
source_filename: amazon-codebuild-batch-delete-builds-output-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codebuild/refs/heads/main/json-schema/amazon-codebuild-batch-delete-builds-output-schema.json\",\n  \"title\": \"BatchDeleteBuildsOutput\",\n  \"description\": \"BatchDeleteBuildsOutput schema from Amazon CodeBuild\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"buildsDeleted\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BuildIds\"\n        },\n        {\n          \"description\": \"The IDs of the builds that were successfully deleted.\"\n        }\n      ]\n    },\n    \"buildsNotDeleted\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BuildsNotDeleted\"\n        },\n        {\n          \"description\": \"Information about any builds that could not be successfully deleted.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codebuild/refs/heads/main/json-schema/amazon-codebuild-batch-delete-builds-output-schema.json
tags:
- Amazon
- AWS
- CI/CD
- Build
- Continuous Integration
- DevOps
- Testing
title: BatchDeleteBuildsOutput
---
