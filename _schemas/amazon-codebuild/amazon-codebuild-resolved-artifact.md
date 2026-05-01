---
description: Represents a resolved build artifact. A resolved artifact is an artifact that is built and deployed to the destination, such as Amazon S3.
layout: schema
name: ResolvedArtifact
properties_list:
- description: ''
  name: type
  type: object
- description: ''
  name: location
  type: object
- description: ''
  name: identifier
  type: object
provider_name: Amazon CodeBuild
provider_slug: amazon-codebuild
schema_file: json-schema/amazon-codebuild-resolved-artifact-schema.json
slug: amazon-codebuild-resolved-artifact
source_filename: amazon-codebuild-resolved-artifact-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codebuild/refs/heads/main/json-schema/amazon-codebuild-resolved-artifact-schema.json\",\n  \"title\": \"ResolvedArtifact\",\n  \"description\": \"Represents a resolved build artifact. A resolved artifact is an artifact that is built and deployed to the destination, such as Amazon S3.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"type\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ArtifactsType\"\n        },\n        {\n          \"description\": \"Specifies the type of artifact.\"\n        }\n      ]\n    },\n    \"location\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The location of the artifact.\"\n        }\n      ]\n    },\n    \"identifier\": {\n      \"allOf\": [\n        {\n          \"$ref\":\
  \ \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The identifier of the artifact.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codebuild/refs/heads/main/json-schema/amazon-codebuild-resolved-artifact-schema.json
tags:
- Amazon
- CI/CD
- Build
- Continuous Integration
- DevOps
- Testing
title: ResolvedArtifact
---
