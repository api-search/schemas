---
description: ListCuratedEnvironmentImagesOutput schema from Amazon CodeBuild
layout: schema
name: ListCuratedEnvironmentImagesOutput
properties_list:
- description: ''
  name: platforms
  type: object
provider_name: Amazon CodeBuild
provider_slug: amazon-codebuild
schema_file: json-schema/amazon-codebuild-list-curated-environment-images-output-schema.json
slug: amazon-codebuild-list-curated-environment-images-output
source_filename: amazon-codebuild-list-curated-environment-images-output-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codebuild/refs/heads/main/json-schema/amazon-codebuild-list-curated-environment-images-output-schema.json\",\n  \"title\": \"ListCuratedEnvironmentImagesOutput\",\n  \"description\": \"ListCuratedEnvironmentImagesOutput schema from Amazon CodeBuild\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"platforms\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EnvironmentPlatforms\"\n        },\n        {\n          \"description\": \"Information about supported platforms for Docker images that are managed by CodeBuild.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codebuild/refs/heads/main/json-schema/amazon-codebuild-list-curated-environment-images-output-schema.json
tags:
- Amazon
- CI/CD
- Build
- Continuous Integration
- DevOps
- Testing
title: ListCuratedEnvironmentImagesOutput
---
