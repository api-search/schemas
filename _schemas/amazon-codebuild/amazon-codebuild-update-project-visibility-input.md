---
description: UpdateProjectVisibilityInput schema from Amazon CodeBuild
layout: schema
name: UpdateProjectVisibilityInput
properties_list:
- description: ''
  name: projectArn
  type: object
- description: ''
  name: projectVisibility
  type: object
- description: ''
  name: resourceAccessRole
  type: object
provider_name: Amazon CodeBuild
provider_slug: amazon-codebuild
schema_file: json-schema/amazon-codebuild-update-project-visibility-input-schema.json
slug: amazon-codebuild-update-project-visibility-input
source_filename: amazon-codebuild-update-project-visibility-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codebuild/refs/heads/main/json-schema/amazon-codebuild-update-project-visibility-input-schema.json\",\n  \"title\": \"UpdateProjectVisibilityInput\",\n  \"description\": \"UpdateProjectVisibilityInput schema from Amazon CodeBuild\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"projectArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NonEmptyString\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the build project.\"\n        }\n      ]\n    },\n    \"projectVisibility\": {\n      \"$ref\": \"#/components/schemas/ProjectVisibilityType\"\n    },\n    \"resourceAccessRole\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NonEmptyString\"\n        },\n        {\n          \"description\": \"The ARN of the IAM role that enables CodeBuild\
  \ to access the CloudWatch Logs and Amazon S3 artifacts for the project's builds.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"projectArn\",\n    \"projectVisibility\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codebuild/refs/heads/main/json-schema/amazon-codebuild-update-project-visibility-input-schema.json
tags:
- Amazon
- AWS
- CI/CD
- Build
- Continuous Integration
- DevOps
- Testing
title: UpdateProjectVisibilityInput
---
