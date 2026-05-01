---
description: UpdateProjectVisibilityOutput schema from Amazon CodeBuild
layout: schema
name: UpdateProjectVisibilityOutput
properties_list:
- description: ''
  name: projectArn
  type: object
- description: ''
  name: publicProjectAlias
  type: object
- description: ''
  name: projectVisibility
  type: object
provider_name: Amazon CodeBuild
provider_slug: amazon-codebuild
schema_file: json-schema/amazon-codebuild-update-project-visibility-output-schema.json
slug: amazon-codebuild-update-project-visibility-output
source_filename: amazon-codebuild-update-project-visibility-output-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codebuild/refs/heads/main/json-schema/amazon-codebuild-update-project-visibility-output-schema.json\",\n  \"title\": \"UpdateProjectVisibilityOutput\",\n  \"description\": \"UpdateProjectVisibilityOutput schema from Amazon CodeBuild\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"projectArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NonEmptyString\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the build project.\"\n        }\n      ]\n    },\n    \"publicProjectAlias\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NonEmptyString\"\n        },\n        {\n          \"description\": \"Contains the project identifier used with the public build APIs. \"\n        }\n      ]\n    },\n    \"projectVisibility\": {\n      \"$ref\"\
  : \"#/components/schemas/ProjectVisibilityType\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codebuild/refs/heads/main/json-schema/amazon-codebuild-update-project-visibility-output-schema.json
tags:
- Amazon
- CI/CD
- Build
- Continuous Integration
- DevOps
- Testing
title: UpdateProjectVisibilityOutput
---
