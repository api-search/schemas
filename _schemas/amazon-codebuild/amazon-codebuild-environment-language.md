---
description: A set of Docker images that are related by programming language and are managed by CodeBuild.
layout: schema
name: EnvironmentLanguage
properties_list:
- description: ''
  name: language
  type: object
- description: ''
  name: images
  type: object
provider_name: Amazon CodeBuild
provider_slug: amazon-codebuild
schema_file: json-schema/amazon-codebuild-environment-language-schema.json
slug: amazon-codebuild-environment-language
source_filename: amazon-codebuild-environment-language-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codebuild/refs/heads/main/json-schema/amazon-codebuild-environment-language-schema.json\",\n  \"title\": \"EnvironmentLanguage\",\n  \"description\": \"A set of Docker images that are related by programming language and are managed by CodeBuild.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"language\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LanguageType\"\n        },\n        {\n          \"description\": \"The programming language for the Docker images.\"\n        }\n      ]\n    },\n    \"images\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EnvironmentImages\"\n        },\n        {\n          \"description\": \"The list of Docker images that are related by the specified programming language.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codebuild/refs/heads/main/json-schema/amazon-codebuild-environment-language-schema.json
tags:
- Amazon
- AWS
- CI/CD
- Build
- Continuous Integration
- DevOps
- Testing
title: EnvironmentLanguage
---
