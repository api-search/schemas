---
description: Information about a Docker image that is managed by CodeBuild.
layout: schema
name: EnvironmentImage
properties_list:
- description: ''
  name: name
  type: object
- description: ''
  name: description
  type: object
- description: ''
  name: versions
  type: object
provider_name: Amazon CodeBuild
provider_slug: amazon-codebuild
schema_file: json-schema/amazon-codebuild-environment-image-schema.json
slug: amazon-codebuild-environment-image
source_filename: amazon-codebuild-environment-image-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codebuild/refs/heads/main/json-schema/amazon-codebuild-environment-image-schema.json\",\n  \"title\": \"EnvironmentImage\",\n  \"description\": \"Information about a Docker image that is managed by CodeBuild.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The name of the Docker image.\"\n        }\n      ]\n    },\n    \"description\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The description of the Docker image.\"\n        }\n      ]\n    },\n    \"versions\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ImageVersions\"\n        },\n        {\n          \"description\"\
  : \"A list of environment image versions.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codebuild/refs/heads/main/json-schema/amazon-codebuild-environment-image-schema.json
tags:
- Amazon
- CI/CD
- Build
- Continuous Integration
- DevOps
- Testing
title: EnvironmentImage
---
