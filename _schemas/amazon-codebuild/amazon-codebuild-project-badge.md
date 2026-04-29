---
description: Information about the build badge for the build project.
layout: schema
name: ProjectBadge
properties_list:
- description: ''
  name: badgeEnabled
  type: object
- description: ''
  name: badgeRequestUrl
  type: object
provider_name: Amazon CodeBuild
provider_slug: amazon-codebuild
schema_file: json-schema/amazon-codebuild-project-badge-schema.json
slug: amazon-codebuild-project-badge
source_filename: amazon-codebuild-project-badge-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codebuild/refs/heads/main/json-schema/amazon-codebuild-project-badge-schema.json\",\n  \"title\": \"ProjectBadge\",\n  \"description\": \"Information about the build badge for the build project.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"badgeEnabled\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Boolean\"\n        },\n        {\n          \"description\": \"Set this to true to generate a publicly accessible URL for your project's build badge.\"\n        }\n      ]\n    },\n    \"badgeRequestUrl\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The publicly-accessible URL through which you can access the build badge for your project. \"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codebuild/refs/heads/main/json-schema/amazon-codebuild-project-badge-schema.json
tags:
- Amazon
- AWS
- CI/CD
- Build
- Continuous Integration
- DevOps
- Testing
title: ProjectBadge
---
