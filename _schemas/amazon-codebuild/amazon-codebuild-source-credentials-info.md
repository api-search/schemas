---
description: Information about the credentials for a GitHub, GitHub Enterprise, or Bitbucket repository.
layout: schema
name: SourceCredentialsInfo
properties_list:
- description: ''
  name: arn
  type: object
- description: ''
  name: serverType
  type: object
- description: ''
  name: authType
  type: object
provider_name: Amazon CodeBuild
provider_slug: amazon-codebuild
schema_file: json-schema/amazon-codebuild-source-credentials-info-schema.json
slug: amazon-codebuild-source-credentials-info
source_filename: amazon-codebuild-source-credentials-info-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codebuild/refs/heads/main/json-schema/amazon-codebuild-source-credentials-info-schema.json\",\n  \"title\": \"SourceCredentialsInfo\",\n  \"description\": \" Information about the credentials for a GitHub, GitHub Enterprise, or Bitbucket repository. \",\n  \"type\": \"object\",\n  \"properties\": {\n    \"arn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NonEmptyString\"\n        },\n        {\n          \"description\": \" The Amazon Resource Name (ARN) of the token. \"\n        }\n      ]\n    },\n    \"serverType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ServerType\"\n        },\n        {\n          \"description\": \" The type of source provider. The valid options are GITHUB, GITHUB_ENTERPRISE, or BITBUCKET. \"\n        }\n      ]\n    },\n    \"authType\": {\n \
  \     \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AuthType\"\n        },\n        {\n          \"description\": \" The type of authentication used by the credentials. Valid options are OAUTH, BASIC_AUTH, or PERSONAL_ACCESS_TOKEN. \"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codebuild/refs/heads/main/json-schema/amazon-codebuild-source-credentials-info-schema.json
tags:
- Amazon
- CI/CD
- Build
- Continuous Integration
- DevOps
- Testing
title: SourceCredentialsInfo
---
