---
description: A set of Docker images that are related by platform and are managed by CodeBuild.
layout: schema
name: EnvironmentPlatform
properties_list:
- description: ''
  name: platform
  type: object
- description: ''
  name: languages
  type: object
provider_name: Amazon CodeBuild
provider_slug: amazon-codebuild
schema_file: json-schema/amazon-codebuild-environment-platform-schema.json
slug: amazon-codebuild-environment-platform
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codebuild/refs/heads/main/json-schema/amazon-codebuild-environment-platform-schema.json\",\n  \"title\": \"EnvironmentPlatform\",\n  \"description\": \"A set of Docker images that are related by platform and are managed by CodeBuild.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"platform\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PlatformType\"\n        },\n        {\n          \"description\": \"The platform's name.\"\n        }\n      ]\n    },\n    \"languages\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EnvironmentLanguages\"\n        },\n        {\n          \"description\": \"The list of programming languages that are available for the specified platform.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codebuild/refs/heads/main/json-schema/amazon-codebuild-environment-platform-schema.json
tags:
- Amazon
- AWS
- CI/CD
- Build
- Continuous Integration
- DevOps
- Testing
title: EnvironmentPlatform
---
